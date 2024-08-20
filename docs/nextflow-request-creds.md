[![Nextflow logo](img/nextflow.svg){: style="height:75px"}](https://www.nextflow.io/)

# **Request Credentials for Uploading a Docker Container**

Before you request credentials, please be sure that you have successfully [built your Docker image locally](nextflow-create-docker.md/#build-your-image-locally-on-top-of-the-base-image), and that you have already [scanned it with Docker Scout](nextflow-create-docker.md/#my-image-passes-the-local-security-scanning). This will reduce the likelihood of needing to re-request credentials for this container.

*Please copy and paste the email template below into a new email and send to [brhsupport@gen3.org](mailto:brhsupport@gen3.org). Please be sure to add the relevant information to the bolded fields.*

------
Hello, User Services,

Please create new temporary AWS credentials to permit me to upload a Nextflow container.

The email address or ORCID I use to log in to BRH is: **[BRH login email here]**

I understand that these credentials will last for 1 hour, once created. If I continue to need access to upload after they expire, I will request new credentials.

Since the credentials will ONLY last 1 hour after creation, you may prefer we send them at a certain time of day. Please **delete which of these do NOT apply**:

* Please generate and send my credentials tomorrow morning
* Please generate and send my credentials in the afternoon
* Please generate and send my credentials ASAP

To ensure prompt attention, I will also ping `nextflow-support` *(please do not use @ for this)* on the Slack channel after I have sent my email.


Thanks!

**[your name]**

------

We will send you the credentials through direct message on Slack, in a link to keep them private.  

Please note: If you receive credentials but you are not able to successfully upload an image before they expire, please ping `nextflow-support` on Slack to let us know we do not need to monitor your submitted image.

[*Continue to Upload Docker Image*](./nextflow-upload-docker.md)
