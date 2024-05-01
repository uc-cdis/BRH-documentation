[![Nextflow logo](img/nextflow.svg){: style="height:75px"}](https://www.nextflow.io/)

# **Overview: Developing and Deploying Containers in Gen3**

![Overview of steps in developing a container and making it available for use in workflows](./img/container-development.png)

**Locally build and test container:**

Gen3 provides several [FedRAMP security-compliant base images](https://github.com/uc-cdis/containers/blob/eec9789a57c5bb196a91f035e4cb069cfaa5abcd/nextflow-base-images/allowed_base_images.txt) that users can pull and customize.

**Request credentials and push container to Gen3 staging:**

Users can email Gen3 to [request short-term credentials](nextflow-request-creds.md) that permit them to authenticate Docker in their terminal to upload the local Docker image to a Gen3 staging repo for security review.

**Container is security-scanned; Gen3 sends approved container URI:**

Gen3 completes the security scan of the container. Typically, the scanning completes within a couple hours; however it takes longer for larger images with more layers. If it is security-compliant, the image is moved to an ECR repo ("approved") from where the container can be run, and Gen3 staff will send a container URI to the user for use in the Nextflow workflows.

If there are problems that make the image non-compliant with security requirements, a report of the vulnerabilities is provided to the user for remediation and resubmission. Users are responsible for resolving image vulnerabilities and resubmitting for scanning.  

**Run workflow using approved container URI:**

In the BRH workspace, use a Nextflow Jupyter notebook to run Nextflow workflows in the approved container using the approved container URI. Some example notebooks can be found [here](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks), and specific examples that use an approved image URI can be found [here](https://github.com/uc-cdis/bio-nextflow/blob/master/nextflow_notebooks/containerized_gpu_workflows/torch_cuda_test/torch_cuda_batch_template.ipynb) and [here](https://github.com/uc-cdis/bio-nextflow/blob/master/nextflow_notebooks/containerized_gpu_workflows/torch_cuda_test/README.md)

---
[*Continue to Create Dockerfile*](./nextflow-create-docker.md)
