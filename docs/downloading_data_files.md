# **Downloading Data Files**

Users can download data files for work in the provided [Workspace][Workspaces page]. Utilizing workspaces leverages CTDS-owned python software development kit (SDK) as well as a cloud-based computing platform.

**Note: accessing data files requires linked access to all FAIR enabled repositories, as described [here][Request study access].**

## Download Data Files into a Workspace with the Python SDK

Users can load data files from a manifest created on the Discovery Page directly into a Workspace.
Below are the steps to do so.

1. Navigate to the [Discovery Page][Discovery page]. Link your accounts to FAIR repositories as described [here][Request study access].

2. Find the study or studies of interest by using the [search features][Discovery page] or the [list of accessible studies][Discovery page].

3. Select the clickable boxes next to the studies.
Click on "Open in Workspace", which will initiate the [Workspace Launcher][Workspaces page].

      ![Select the studies and click "Open In Workspace".][img open data in wksp]

4. The Workspace will be prepared and the selected data will be made available via a manifest placed in a time/date stamped directory in the following path: pd/data/brh.data-commons.org/exported-manifest-(time/date stamp) Please do not navigate away from this page until the download is complete. Created directory may take several minutes to load.

      ![Workspace manifest downloaded to pd directory][img workspace manifest]

5. Once loaded, users can navigate into the directory and access either the manifest or an automatically generated notebook (e.g., data.ipynb) with instructions to download the data. Users should note that the gen3-sdk is utilized in this notebook and directory to download data.

      ![The manifest and a notebook are available in the pd directory][img data notebook]

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
[Workspace timeout]: https://brh.data-commons.org/dashboard/Public/index.html#AutomaticWorkspaceShutdown
[img wksp register]: ./img/brh-portal-login-strides.png
[img open data in wksp]: ./img/open_data_in_workspace.png
[img workspace manifest]: ./img/open_in_workspace_manifest_path.png
[img data notebook]: ./img/open_in_workspace_datanb.png
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
[img profile]: ./img/profile_access.png
[Download Data Files into a Workspace with the Python SDK]: https://brh.data-commons.org/dashboard/Public/index.html#OpeninWorkspacefromDiscovery
[GitHub]: https://docs.github.com/en
[Data Availability Options]: https://brh.data-commons.org/dashboard/Public/index.html#DataAvailabilityOptions
[Find Study Metadata]: https://brh.data-commons.org/dashboard/Public/index.html#FindStudyMetadata
[Download data files]: https://brh.data-commons.org/dashboard/Public/index.html#DownloadingDataFiles
[eRA]: https://era.nih.gov/
[Jupyter]: https://jupyter.org/
[Profile page]: https://brh.data-commons.org/identity
[BRH login]: https://brh.data-commons.org/login
[BRH Workspace]: https://brhstaging.data-commons.org/workspace
[BRH Platform]: https://brh.data-commons.org/
[BRH Discovery]: https://brh.data-commons.org/discovery
[Gen3.org]: https://gen3.org/
[img BRH logo]: ./img/brh-logo.png
[img Gen3 logo]: ./img/gen3blue.png
[Register for workspaces]: workspace_registration.md
[Login page]: loginoverview.md
[Request study access]: how_to_check_request_access.md
[Discovery page]: discovery_page.md
[Workspaces page]: workspace_page.md
[Profile page]: profile_page.md
