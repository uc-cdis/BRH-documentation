[![Nextflow logo](img/nextflow.svg){: style="height:75px"}](https://www.nextflow.io/)

# **Tutorial Nextflow Workflows**

We have a collection of notebooks using Nextflow in Gen3 here: [https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks)

Before you start executing any tutorial notebooks, review the information in the [Get Set](#get-set-download-necessary-credentials-and-software) section.  

## **Get set: Download necessary credentials and software**

Be ready to execute the tutorial workflows below by gathering credentials and installing necessary software.  

### **Get and replace placeholder values from the Nextflow config**

You can find the values to replace the placeholders in the`queue`, `jobRole` and `workDir` fields in the `nextflow.config` file in your Nextflow workspace (this is found in `/data directory`, unless you have moved it to the `/pd`). These placeholder values will need to be replaced in each of the various tutorial Nextflow notebooks.

Note that you should only copy/paste the value to replace `placeholder` for each field; do not copy/paste larger sections of the nextflow config, or there could be indentation problems that interfere with the code.

### **MIDRC credentials**

To download GUIDs in the workspace, you will first need to generate a MIDRC credentials on the profile page of the [MIDRC portal](https://data.midrc.org/). For this, please go to [data.midrc.org](https://data.midrc.org/), click on the user icon in the right corner (#1), and open the Profile page (#2). Click on Create API Key (#3). A pop-up window will appear with the key. If you scroll down slightly, you can see the button to download the credentials as a JSON. Credentials are valid for 1 month.

![Screenshot showing how to find and save MIDRC credentials](./img/MIDRC-credentials.png)

## **Example Nextflow notebooks**

### **Notebooks with no containers**

There are several general Nextflow notebooks that do not use containers at all. If you're new to nextflow and just want to get started with workflow commands, try these notebooks: [https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/non_containerized_nextflow_workflows](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/non_containerized_nextflow_workflows)

### **Notebooks using containers**

We have several [containerized notebooks using CPU](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_cpu_workflows), and other [containerized notebooks using GPU](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_gpu_workflows).  

#### Notebooks using CPU

You can find the directory with containerized notebooks using CPU here: [https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_cpu_workflows](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_cpu_workflows)

Some use cases in this directory include:

* **Cancer use case:** The `chip_cancer` [example tutorial here](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_cpu_workflows/chip_cancer) includes a Dockerfile, a requirements file, a Nextflow notebook, a collection of python scripts, and a README.
* **DICOM metadata extraction use case:** The `midrc_batch_demo` [example tutorial here](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_cpu_workflows/midrc_batch_demo) includes a Dockerfile, a requirements file, two Nextflow notebooks, a collection of python scripts, and a README.

#### Notebooks using GPU

You can find the directory with containerized notebooks using GPU here: [https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_gpu_workflows](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_gpu_workflows)

Some use cases in this directory include:

* **Pytorch/cuda test simple use case:** The `torch_cuda_test` [example tutorial here](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_gpu_workflows/torch_cuda_test) includes a Dockerfile, a requirements file, a Nextflow notebook, a simple python script, and a README.
* **COVID Challenge 2022 use case:** The `covid_challenge_container` [example tutorial here](https://github.com/uc-cdis/bio-nextflow/tree/master/nextflow_notebooks/containerized_gpu_workflows/covid_challenge_container) includes a Dockerfile, a requirements file, a Nextflow notebook, a python script, and a README.
