# **Monitor Compute Usage with a Persistent Pay Model**

## Where can you see your usage?

You can see and monitor your compute usage in two places:

1. Workspace Page
2. Workspace Account Manager

Two important notes:  

* This usage reporting is only available for users with a persistent paymodel; it is not available for the trial access accounts.  
* Usage reported in either of these places generally **does not immediately update as you use the workspace**. AWS reports updated usage about three times per day.  

### 1. Monitor usage on the **Workspace page**

You can see your total usage for any active paid accounts by logging in to the [BRH platform][BRH Platform], clicking on [Workspace][BRH Workspace] (#1), then clicking on Account Information (#2 in the upper left). You can see your total usage and your spending limit (see arrows).

If you have more than one funded workspace account, you can use the dropdown (#3) to select different active pay models and view their usage and spending limits.

![Monitor your workspace compute usage with information on the Workspace page.][img monitor wkspc pg]

### 2. Monitor usage on the **Workspace Account Manager**

You can see your usage details on the [Workspace Account Manager][Wksp account mgr] Accounts page (#4 in the image above).

After logging in, you will be on the Accounts page. There are different tables for each of the three persistent pay models. Find the table for the persistent pay model account you want to monitor, then look for the active account line in that table.

The table includes 4 columns relevant for monitoring usage (these are highlighted in the image below):

* **Total Usage:** This column reports on your compute usage for this account as of the most recent AWS report.
* **Compute Purchased (or STRIDES Credits):** This is the total purchase amount you have made for this account. For STRIDES Credits accounts, this is the total amount of credit you were awarded.

The soft and hard limit columns deserve their own section; see below.

## Hard and Soft Limits

You can see your hard and soft limits (highlighted in yellow below) in the tables on the [Workspace Account Manager][Wksp account mgr] Accounts page. They each have a column:

* **Soft Limit:** This is the limit at which an alert will be triggered for you that you are approaching the spending limit for the account. For STRIDES accounts, users can edit this column to set the alert threshold. For OCC Direct Pay, the soft limit is set in accordance with your Direct Pay User Agreement (signed during Direct Pay BillingID setup).

* **Hard Limit:** This is the limit at which a workspace VM will be immediately terminated and the workspace account will be shut down such that no VMs can be launched with it. For STRIDES accounts, users can edit this column to set the threshold at which the account becomes inactive. For OCC Direct Pay, the hard limit is set in accordance with your Direct Pay User Agreement (signed during Direct Pay BillingID setup).

![Monitor your workspace compute usage, and see your hard and soft limits, on the Workspace Account Manager.][img monitor wkspc acct mgr]

[*What happens when you exceed your funding for a workspace account?*][Exceed funding]

<!-- Images -->
[img BRH Admin Portal]: ./img/brh-portal-login.png
[img BRH logo]: ./img/brh-logo.png
[img monitor wkspc pg]: ./img/monitor-workspace-pg.png
[img monitor wkspc acct mgr]: ./img/monitor-workspace-acct-mgr.png


<!-- Links -->
[BRH Discovery]: https://brh.data-commons.org/discovery
[BRH login]: https://brh.data-commons.org/login
[BRH Platform]: https://brh.data-commons.org/
[BRH Workspace Acct Mgr]: https://brh-portal.org/
[BRH Workspace]: https://brhstaging.data-commons.org/workspace
[Data Availability Options]: https://brh.data-commons.org/dashboard/Public/index.html#DataAvailabilityOptions
[Discovery page]: 08-discovery_page.md
[Download Data Files into a Workspace with the Python SDK]: https://brh.data-commons.org/dashboard/Public/index.html#OpeninWorkspacefromDiscovery
[Download data files]: https://brh.data-commons.org/dashboard/Public/index.html#DownloadingDataFiles
[eRA]: https://era.nih.gov/
[Find Study Metadata]: https://brh.data-commons.org/dashboard/Public/index.html#FindStudyMetadata
[Gen3.org]: https://gen3.org/
[GitHub]: https://docs.github.com/en
[Jupyter]: https://jupyter.org/
[Login page]: 06-loginoverview.md
[OCC processing stages]: https://payments.occ-data.org/processing-stages/
[pd link]: https://uc-cdis.github.io/BRH-documentation/09-workspace_page/#guideline-to-get-started-in-workspaces
[Register for workspaces]: 05-workspace_registration.md
[Request study access]: 07-how_to_check_request_access.md
[STRIDES]: https://datascience.nih.gov/strides
[Exceed funding]: 16-usage_exceeds_funding.md
[Workspaces page]: 09-workspace_page.md
[BRH wksp access req form]: https://brh.data-commons.org/workspace/request-access
[Wksp account mgr]: https://brh-portal.org/
[Req new wksp]: https://brh-portal.org/request-workspace
[OCC Payment Portal]: https://payments.occ-data.org/
[Payment Portal Profile]: https://payments.occ-data.org/profile/
[OCC Request BillingID]: https://payments.occ-data.org/request-billingid/
