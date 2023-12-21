[![Nextflow logo](/img/nextflow.svg){: style="height:75px"}](https://www.nextflow.io/)

# **Pushing Container Images to AWS ECR**

### Overview
This guide is for external users who have received temporary credentials granting access to push container images to a specific AWS Elastic Container Registry (ECR) repository.

### Prerequisites
- [Docker](https://www.docker.com/get-started/) installed on your local machine.
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) installed locally
- Temporary AWS credentials provided by the User Services team.
- The URI of the ECR repository you have been given access to (should have been shared with you along with the AWS credentials)
- A container you want to push.

### Timing
Your temporary AWS credentials only lasts for 1 hour from when they were created; User Services should have provided an expiration time when sharing the credentials with you. You must fully complete the push to ECR before they expire, or you will need to request new credentials from User Services.

### Set AWS Environment Variables:
Before you can push your Docker image to the ECR repository, you need to configure the AWS CLI with the temporary credentials you received. Here's how you can do that:

 Replace `< AccessKeyId >`, `< SecretAccessKey >`, and `< SessionToken >` with the credentials provided to you.

      export AWS_ACCESS_KEY_ID=<AccessKeyId>
      export AWS_SECRET_ACCESS_KEY=<SecretAccessKey>
      export AWS_SESSION_TOKEN=<SessionToken>

> Note: the variables are set only as long as the terminal is open; export the variables again if you close and open a new terminal.

### Verify Configuration:
Run `aws sts get-caller-identity` to verify that your CLI is using the temporary credentials.

### Logging in to ECR
Use the AWS CLI to retrieve an authentication token and authenticate your Docker client to your registry.

     aws ecr get-login-password --region <region> | docker login --username AWS --password-stdin <repositoryUri>

Replace `< region >` with `us-east-1`, and `< repositoryUri >` with the URI of the ECR repository you've been given access to.

## Pushing Your Docker Image
### Tag Your Docker Image:
Tag your local Docker image with the ECR repository URI and the image tag you want to use.

     docker tag <local-image>:<local-tag> <repositoryUri>:<image-tag>

Replace `< local-image >` with the name of your local Docker image and `< local-tag >` with the tag you want to push.
> If you're not sure what your local image and tag names are, you can run `docker images` in your terminal. It will provide a list of all your saved docker images. The column called `REPOSITORY` is the local image name. The column called `TAG` is the local tag name for this image.

Replace `< repositoryUri >` with the ECR repository URI provided by User Services, and `< image-tag >` with  the image tag name you want to use in your ECR.
> Important note: If you do not want the most-recently-pushed image to replace an earlier version with the same tag in your ECR, image-tags should be unique.
> For example, you create an image with an image-tag `batch-poc`. If you later push another image to `< repositoryUri >:batch-poc`, it will overwrite the previous version of the image in your ECR (you will only have 1 container with the tag "batch-poc").
> If you do not want to overwrite, you can use versioned image-tags. For example: `batch-poc-1.0`, and then `batch-poc-1.1`.
> If you want to replace previous versions of your container, you can use the same image-tag.

### Push the Image:
Push the tagged image to the ECR repository.

     docker push <repositoryUri>:<image-tag>

If the **push is successful**, you will see various "layer 1" "layer 2" etc outputs, and it will indicate progress in pushing. This can take minutes, depending on how large your container is.

If the **push fails**, you will get a message about "Waiting for layer". This usually means it cannot find the repository, so double-check that there is no typo, and that you have set your [AWS environment variables](#set-aws-environment-variables) since you opened the terminal most recently.

### Completion
Once the push completes, your Docker image will be available in the ECR repository. It will be scanned, and if it's safe, CTDS will move it to the nextflow-approved repo. When it's available in nextflow-approved, User Services will share a docker URI that looks something like this:
`143731057154.dkr.ecr.us-east-1.amazonaws.com/nextflow-approved/< your username >:< image-tag >`. You can then use this new URI to run workflows with your container.

## Support
If you encounter any issues or require assistance, please reach out to the User Services team that provided you with the temporary credentials, or brhsupport@datacommons.io, or reach out on Slack.
