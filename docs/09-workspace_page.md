# **Workspaces**

**To use the workspace, users must register for workspace accounts to use the workspaces, as described on the [Workspace Registration page][Register for workspaces].**

BRH workspaces are secure data analysis environments in the cloud that can access data from one or more data resources. By default, Workspaces include Jupyter notebooks, Python and R, but can be configured to host virtually any application, including analysis workflows, data processing pipelines, or data visualization apps.

> New to Jupyter? Learn more about the popular tool for data scientists on [Jupyter.org][Jupyter] (disclaimer: CTDS is not responsible for the content).

## Guideline to get started in Workspaces

Once users have access to workspaces, use this guide below to get started with analysis work in workspaces.

1. Users need to log in via [https://brh.data-commons.org/login][BRH login] to access workspaces.

2. After navigating to [https://brh.data-commons.org/workspace][BRH Workspace], users will discover a list of pre-configured virtual machine (VM) images, as shown below.

      ![Available workspaces on BRH][img workspaces]

      * **(Generic) Jupyter Notebook with R kernel:** Choose this VM if you are familiar with setting up Python- or R-based Notebooks, or if you just exported one or multiple studies from the Discovery Page and want to start your custom analysis.
      * **Tutorial Notebooks:** Explore our [Jupyter Notebook tutorials][BRH tutorial notebooks] written in Python or R, which pull data from various sources of the Biomedical Research Hub to leverage statistical programs and data analysis tools.
         * [JCOIN MOUD Accessibility Analysis][JCOIN MOUD]
         * [Changes in Opiod Treatment Policy During COVID-19][Opiod Treatment Policy]
         * [Gene Expression Analysis of Project TCGA-CHOL][Project TCGA-CHOL]
         * [Proteome Data Commons (PDC) Clustergram][PDC Clustergram]
         * [MIDRC CT Scan][MIDRC CT Scan]
         * [Data Exploration using Python of Framingham Heart Study Teaching Dataset][Python Framingham]
         * [Data Exploration using R of Framingham Heart Study Teaching Dataset][R Framingham]
         * [Data Exploration of CAMP Study Teaching Dataset][CAMP Study]
         * [Canine Data Commons FASTQ Reader][Canine Data Commons]
         * [MIDRC Open-R1 Clinical Data Analysis][MIDRC Open-R1]
         * [JCOIN Tracking Opioid Stigma][JCOIN Opioid Stigma]
         * [Cox Model Implementation using ACTT Data from NIAID Clinical Trials Data Commons][Cox Model ACTT Data]
         * [Identify Prostate Cancer Biomarker using Machine Learning][Prostate Cancer Biomarker]
         * [Identification of Potential Drug Targets of Inflammatory Bowel Disease][Drug Targets of IBD]

3. Click “Launch” on any of the workspace options to spin up a copy of that VM. The status of launching the workspace is displayed after clicking on “Launch”. Note: Launching the VM may take several minutes.

      ![Screenshot of the launch status of the workspace][img Workspace launch status]

4. After launching, the home folders are displayed. One of these folders is the user's persistent drive ("/pd").

      ![Workspace home folder, including the /pd directory][img Workspace Data Folder]

5. Select the /pd folder. New files or licenses should be saved in the the /pd directory if users need to access them after restarting the workspaces. Only files saved in the /pd directory will remain available after termination of a workspace session.

      ![Screenshot of the /pd folder][img PD folder]

      * **Attention:** Any personal files in the folder “data” will be lost. Personal files in the directory /pd will persist.
      * Do not save files in the "data" or “data/brh.data-commons.org” folders.
      * The folder “brh.data-commons.org” in the “data” folder will host the data files you have exported from the Discovery Page.

6. Start a new notebook under “Notebook” in the Launcher tab. Click the tiles in the launcher and choose between Python 3 or R Studio as the base programmatic language. *Note: You can open and run multiple notebooks in your workspace. However, the generic, tutorial and nextflow workspace images are currently separate docker images, so there is no functionality to combine them or run nextflow in the tutorial or generic images. This may be available in the future, after further testing and development activities.*

      ![Start a new notebook under “Notebook” in the Launcher tab][img New Notebook]

7. **Experiment away!** Code blocks are entered in cells, which can be executed individually or all at once. Code documentation and comments can also be entered in cells, and the cell type can be set to support Markdown.

      Results, including plots, tables, and graphics, can be generated in the workspace and downloaded as files.

8. Do not forget to terminate your workspace once your work is finished. Unterminated workspaces continue to accrue computational costs. **Note, that Workspaces automatically shut down after 90 minutes of [idle time][Workspace timeout].**

      ![Screenshot for terminating your workspace][img Terminate workspace]

Further reading: read more about how to download data files into the Workspaces [here][Download data files].

## Upload, save, and download Files/Notebooks

Users can **upload** data files or Notebooks from the local machine to the home directory by clicking on “Upload” in the top left corner. Access the uploaded content in the Notebook (see below).

![Upload data files or Notebooks to the workspace by clicking on “Upload” in the top left corner.][img workspace upload]

Then **run** in the cells, for example:

`import os`

`import pandas as pd`

`os.chdir('/data')`

`demo_df = pd.read_csv('/this_is_a_demo.txt', sep='\t')`

`demo_df.head()`

Users can **save** the notebook by clicking "File" - "Save as", as shown below.

![Save the notebook under “File” - "Save Notebook as"][img Notebook save]

Users can **download** notebooks by clicking "File" - "Download", as shown below. Download the notebook, for example, as ".ipynb".

![Download notebook][img download notebook]

## Environments, Languages, and Tools

The following **environments** are available in the workspaces:

* Jupyter Lab
      ![Jupyter logo][img Jupyter logo]

The following **programmatic languages** are available in Jupyter Notebooks:

* R
* Python 3

The following **tools** are available in Jupyter Notebooks:

* GitHub ([read GitHub documentation][GitHub])

## Python 3 and R in Jupyter

Both Python 3 and R are available in Jupyter Notebooks.

Users can expect to be able to use typical Python or R packages, such as PyPI or CRAN. For Python and R, users can start a new notebook with a tile under "Notebook", as shown below.

![Find Python 3 or R when starting a new notebook under “New”.][img New Notebook]

## Automatic Workspace Shutdown

**Warning:** When a BRH Workspace reaches the STRIDES Credits limit for STRIDES Credits Workspaces, or reaches the Hard Limit for STRIDES Grant Workspaces, the Workspace will be automatically terminated. Please be sure to save any work before reaching the STRIDES Credit or Hard Limit.

**Warning:** Workspaces will also automatically shut down after 90 minutes of idle time. A pop-up window will remind users to navigate back to the workspaces page in order to save the data.

![2' warning for shutdown for workspace][img Workspace shutdown 2']

<!-- Links and Images -->
[img login]: ./img/brh-login.png
[img req access]: ./img/profile_login_other_commons.png
[img Discovery study page]: ./img/discovery_study_page.png
[img Yes access]: ./img/access_YES.png
[img Login other commons]: ./img/profile_login_other_commons.png
[img Discover grid]: ./img/grid_discovery_color_080322.png
[img Discovery features]: ./img/discovery_features_080322.png
[img Discovery Study page metadata]: ./img/discovery_study_page_datafiles.png
[img Workspaces access request]: ./img/workspace_access_form.png
[img Workspace access success]: ./img/workspace_access_success.png
[img workspace upload]: ./img/workspace_upload_080322.png
[img Terminate workspace]: ./img/workspace_terminate_2.png
[Workspace timeout]: 09-workspace_page.md
[img wksp register]: ./img/brh-portal-login-strides.png
[STRIDES]: https://datascience.nih.gov/strides
[img BRH Admin Portal]: ./img/brh-portal-login.png
[img BRH portal request]: .img/brh-portal-request.png
[img STRIDES payment]: ./img/brh-portal-options.png
[img STR grant]: ./img/brh-portal-strides-grant.png
[img STR credit]: ./img/brh-portal-strides-credits.png

[img login]: ./img/brh-login.png
[img req access]: ./img/profile_login_other_commons.png
[img workspaces]: ./img/workspace_flavors_080322.png
[img Workspace launch status]: ./img/workspace_launch.png
[img Workspace Data Folder]: ./img/workspace_data_folder_080322.png
[img PD folder]: ./img/workspace_pd_folder_080422.png
[img New Notebook]: ./img/workspace_new_080322.png
[img Notebook save]: ./img/workspace_notebook_save_080322.png
[img download notebook]: ./img/workspace_notebook_download_080422.png
[img Jupyter logo]: ./img/workspace_jupyter_logo.png
[img Workspace shutdown 2']: ./img/workspace_shutdown_sign_2.png
[GitHub]: https://docs.github.com/en
[Data Availability Options]: https://brh.data-commons.org/dashboard/Public/index.html#DataAvailabilityOptions
[Find Study Metadata]: https://brh.data-commons.org/dashboard/Public/index.html#FindStudyMetadata
[Download data files]: 11-downloading_data_files.md
[Jupyter]: https://jupyter.org/
[Profile page]: https://brh.data-commons.org/identity
[BRH login]: https://brh.data-commons.org/login
[BRH Workspace]: https://brhstaging.data-commons.org/workspace
[BRH tutorial notebooks]: https://brh.data-commons.org/resource-browser
[BRH Platform]: https://brh.data-commons.org/
[BRH Discovery]: https://brh.data-commons.org/discovery
[Gen3.org]: https://gen3.org/
[img BRH logo]: ./img/brh-logo.png
[img Gen3 logo]: ./img/gen3blue.png
[Register for workspaces]: 05-workspace_registration.md
[Login page]: 06-loginoverview.md
[Request study access]: 07-how_to_check_request_access.md
[Discovery page]: 08-discovery_page.md
[Workspaces page]: 09-workspace_page.md
[Profile page]: 10-profile_page.md
[JCOIN MOUD]: https://brh.data-commons.org/dashboard/Public/notebooks/JCOIN_MOUD_accessibility_jupyter_notebook_BRH.html
[Opiod Treatment Policy]: https://brh.data-commons.org/dashboard/Public/notebooks/JCOIN_PDAPS_Public_Policy_Changes.html
[Project TCGA-CHOL]: https://brh.data-commons.org/dashboard/Public/notebooks/GDC_TCGA-CHOL_RNA_analysis_BRH_040722.html
[PDC Clustergram]: https://brh.data-commons.org/dashboard/Public/notebooks/PDC_clustergram.html
[MIDRC CT Scan]: https://brh.data-commons.org/dashboard/Public/notebooks/MIDRC_CT_Scan_Demo.html
[Python Framingham]: https://brh.data-commons.org/dashboard/Public/notebooks/BDCat_Biolincc_Framingham_study_exploration.html
[R Framingham]: https://brh.data-commons.org/dashboard/Public/notebooks/BDCat_Framingham_study_exploration_R.html
[CAMP Study]: https://brh.data-commons.org/dashboard/Public/notebooks/BDCat_CAMP_study_exploration_notebook.html
[Canine Data Commons]: https://brh.data-commons.org/dashboard/Public/notebooks/canine_datacommons_fastq_reader.html
[MIDRC Open-R1]: https://brh.data-commons.org/dashboard/Public/notebooks/MIDRC_Clinical_Data_Demo.html
[JCOIN Opioid Stigma]: https://brh.data-commons.org/dashboard/Public/notebooks/JCOIN_Tracking_Opioid_Stigma.html
[Cox Model ACTT Data]: https://brh.data-commons.org/dashboard/Public/notebooks/ACTT1_accessclinical_notebook.html
[Prostate Cancer Biomarker]: https://brh.data-commons.org/dashboard/Public/notebooks/TCGA_PRAD_Analysis.html
[Drug Targets of IBD]: https://brh.data-commons.org/dashboard/Public/notebooks/IBD_notebook.html
