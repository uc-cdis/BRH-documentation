# Workspace Accounts - Trial and Persistent Pay Models (STRIDES, Direct Pay)

## Four Different Pay Models for BRH Workspace Accounts

We have 4 different pay models for workspace accounts:

* **Trial Access** (free for user, limited to 2 months)
* **OCC Direct Pay** (persistent pay model paid by credit card through OCC Payment Portal)
* **STRIDES Grant/Award Funded** (persistent pay model paid by organizations with NIH grant funds)
* **STRIDES Credits** (persistent pay model paid directly by NIH)

Instructions for requesting funding for each pay model are provided below.

> **Please Note:**

> * The process for granting access for a workspace account can take **2-4 weeks for NIH STRIDES**, although it may also be faster.
> * The account from each different paymodel will have its own workspace storage directory (`/pd`; [read about `/pd` here][Workspaces page]); **data is not shared between accounts with different funding types**. However, you can import and export data among accounts as long as they are active and have funding.

## Request Trial Access
Trial Access is granted for 2 months when you request access to the BRH Workspace page. The instructions for requesting workspace access are on the [Workspace Registration page][Register for workspaces]. Note that your trial access will become inactive as soon as you have a workspace account funded through a persistent paymodel.

## Requesting Funding for Workspace Accounts Through Any Persistent Pay Model

1. Once they have access to the Workspace page, users can request a workspace account by first logging to BRH (#1), going to the Workspace page (#2), then clicking the Workspace Account Manager link (#3). Click "Log in" and "Yes, I authorize" to open the portal in a new tab.

      ![Step by step navigation to open Workspace Account Manager][img open Workspace AM]

      *Some STRIDES users may receive an invitation via email to register for an NIH STRIDES workspace account. These users can also click the link in the invitation email to get to the [BRH Workspace Account Manager][BRH Workspace Acct Mgr].*


2. In the BRH Workspace Account Manager, users can see their persistent workspace accounts and any available credits or funds in the accounts. If you only have trial access, you will not see any active accounts.

      To request a workspace account with a persistent paymodel, click the "Request New Workspace" button.

      ![BRH Workspace Account Manager page to request new workspace account][img BRH portal request]


3. Choose from any of the 3 persistent pay model funding options: a) STRIDES Grant/Award Funded; b) STRIDES Credits; or c) OCC Direct Pay to request a funded workspace account.

      ![Options for persistent paymodels to fund workspaces][img Request persistent pay]

### **OCC Direct Pay** Funded Workspace Account

The **OCC Direct Pay** form can be selected if a user wants to pay with a personal or organizational credit card. OCC Direct Pay only requires a valid credit card.

Funding a workspace account with OCC Direct Pay has 2 major parts:

1. Request BillingID
2. Use BillingID to provision Direct Pay funds for the Workspace Account

#### Request BillingID

1. Go to [**https://payments.occ-data.org**][OCC Payment Portal] or click on the Payment Portal link (red arrow below) on the OCC Direct Pay tab for the workspace account request form.

      ![Screenshot showing where the OCC Payment Portal link can be found in the OCC Direct Pay form][img Link to pay Portal]

2. Create an account for the OCC Payment Portal: Under Create Account, enter your email address and click “Request Token”. *Note: This should be the email address you use to log into BRH; Direct Pay is not currently compatible with ORCID login. If you already logged in with ORCID to request a workspace account, please log out and authenticate with either the InCommon or Google option. Please monitor this address, as relevant alerts will be sent here.*
3. You will receive an email with a 6-digit token within a couple minutes of your request. It may go to spam, so watch the Spam folder, as well.
4. Copy your token from your email. Paste it into the Enter Token field on the OCC Payment Portal. Click Sign In. *(Note: You will be asked to enter a token at each log-in.)*
5. Successful sign-in will open a [Profile page][Payment Portal Profile] for your account on the OCC Payment Portal. When you first create your account on the payment portal, you will not have any access requests.

      ![Screenshot showing payment portal profile page, showing no access requests at the bottom.][img Pay Portal Profile]

6. Click the “request access” button. The form shown below will open. Complete the form and click Submit.

       ![Request Access form on OCC Payment Portal][img request BillingID]

       For Role, indicate your role within your organization/institution. If you don't have an institutional affiliation, you can put "independent data analyst"

7. Once the form is submitted, a message will appear indicating successful submission. You will also receive an email (again, check spam).
8. If you return to the [Profile page][Payment Portal Profile] in the OCC Payment Portal now, you’ll see there is an active request in the table at the bottom. Click “Check Status” to view progress on the steps toward final approval and provisioning of your request. You can view what happens at each stage of processing here: [https://payments.occ-data.org/processing-stages/][OCC processing stages].
9.  When you click Check Status, you can see the progress of your request. At first, you will see that they are processing your request (indicated by an orange color). Once OCC finishes processing your access request, you will receive 2 emails, and the progress tracker at the bottom will show that Submit Access Request is completed (green). Complete E-Doc is now colored orange. The first email indicates that your access request status has progressed, and the second email has a link to an electronic document.

      >>>
      **Important: Review the Agreement carefully to understand the terms.**
      PLEASE READ THIS DOCUMENT VERY CAREFULLY BEFORE SIGNING!
      This document presents the terms governing how your Direct Pay funds will be allocated, among other things. Be sure you understand all the terms before you sign and submit.
      If you have any questions or concerns about the terms and conditions, please email [billing@occ-data.org][OCC billing] before you sign.
      >>>

      Once you submit the signed document, allow 1 business day to finish processing receipt of the signed document and update your progress tracker. You will receive an email when processing is complete.

      But, you will receive an email quickly confirming that the document has been signed and providing a link to download the signed document for your records. If you do not receive that within 5 minutes (be sure to check your spam folder), please return to the document and verify that you fully signed and submitted the document. Please save the document so you can reference it as needed.

10. When your request has been fully approved, the “Received Approval” step will be green, you’ll receive an email, and your BillingID field will have been populated on the [Profile page][Payment Portal Profile] of the OCC Payment Portal.

You may now use your BillingID to provision a Direct Pay workspace account in BRH.

#### Use BillingID to provision Direct Pay funds for the Workspace Account

*Note 1: Before you request a workspace account through any persistent pay model (eg, Direct Pay, STRIDES), be sure to backup all data in your `/pd` for your workspace. Once your persistent pay model is funded, you will no longer have access to the `/pd` used during trial access. ([What’s a `/pd`?][pd link])*

1. Copy your BillingID from your [User Profile page][Payment Portal Profile] in the OCC Payment Portal.
2. Return to the [Workspace Account Manager][BRH Workspace Acct Mgr], and click Request New Workspace to open the [Workspace Account Request Form][Req new wksp].
3. Click the OCC Direct Pay tab.
4. Paste your BillingID in the field, and enter the first 3 characters of the email address associated with your BillingID (For example, if your email was john.smith@gmail.com, you would enter “joh”)
5. Click Confirm BillingID. Once your BillingID is confirmed, the bottom part of the form will open to allow you to enter the details for provisioning your account.
6. Be sure to check the box that says that you agree to be invoiced. The amount of the invoice is taken from the value you entered when you made your access request on the [Payment Portal][OCC Payment Portal].
      * Enter a title for your project and a brief summary. This is to be used to help you keep track of your requests in case you have multiple accounts for different projects.
      * Identify whether your workspace use is personal or organizational.
      * Indicate whether you have a credit card you are allowed to use to pay for provisioning the workspace account. If your workspace is personal and you have any credit card, the answer will be yes. If your workspace is organizational - make sure you are not using a departmental card or similar without permission.
      * Indicate what role you have as a researcher on this project.

       ![OCC Workspace Account Request form on BRH Workspace Account Manager][img Request Direct Pay workspace]

7. Once you submit this form, you will receive an email with the invoice. (Allow 1 business day for this to be sent.) There will be a secure link in the invoice to submit your credit card information and pay the invoice. When you pay the invoice, OCC will apply the funds, create an AWS account for this project’s workspace, and send that information to BRH to provision your account. Allow 1 business day for this after you have signed the form. You will receive an email when your account is set up and ready to be used in your workspace.

      When you submit this form, you will also see a new entry in the OCC Direct Pay Accounts table in the [Workspace Account Manager][Workspace Acct Mgr]. The request status for your request will be Pending until the invoice is paid and the account is finalized.

8. Once your Direct Pay request is funded, your workspace will be shown as Active on the Request Status column in the [Workspace Account Manager][Workspace Acct Mgr].

### **STRIDES Grant/Award** Funded Workspace Account

The **STRIDES Grant/Award Funded** form can be selected if researchers have received NIH funding (e.g. a grant, contract, cooperative agreement, or other transaction agreement) and intend to use these funds for the BRH workspace account. With this option, the researchers' organization will be responsible for payment.

![Request form if you're using STRIDES grant or award funding][img STR grant]

Submit the request form. Note that the process of granting access for a workspace account **can take 2-4 weeks** and users will be notified by email. Following approval, users will see the provisioned workspace account in the [BRH Workspace Accounts Manager][BRH Workspace Acct Mgr].

### **STRIDES Credits** Funded Workspace Account

Select the **STRIDES Credits** form to request credits from the NIH STRIDES Initiative for the BRH Workspace account. With this option, once the request is approved, a new account with a set spending limit of will be provisioned by NIH directly for usage.

![Request form if you're using STRIDES credits][img STR credit]

Submit the request form. Note that the process of granting access for a workspace account **can take 2-4 weeks** and users will be notified by email. Following approval, users will see the provisioned workspace account in the [BRH Workspace Accounts Manager][BRH Workspace Acct Mgr].

## What is the NIH STRIDES Initiative?

The **NIH STRIDES** initiative (NIH **S**cience and **T**echnology **R**esearch **I**nfrastructure for **D**iscovery, **E**xperimentation, and **S**ustainability) can provide funding for BRH Workspace Accounts. The NIH STRIDES Initiative enables researchers with NIH grants to cost-effectively leverage the use of cloud environments by partnering with commercial providers, such as Amazon Web Services.

By leveraging the STRIDES Initiative, NIH and NIH-funded institutions can begin to create a robust, interconnected ecosystem that breaks down silos related to generating, analyzing, and sharing research data.

NIH-funded researchers with an active NIH award may take advantage of the STRIDES Initiative for their NIH-funded research projects. Eligible researchers include NIH intramural researchers and awardees of NIH contracts, other transaction agreements, grants, cooperative agreements, and other agreements. More information on NIH STRIDES options and how to gain access can be found [here][STRIDES].



<!-- Images -->
[img BRH Admin Portal]: ./img/brh-portal-login.png
[img BRH logo]: ./img/brh-logo.png
[img BRH portal request]: ./img/brh-portal-request.png
[img data notebook]: ./img/open_in_workspace_datanb.png
[img Discover grid]: ./img/grid_discovery_color_080322.png
[img Discovery features]: ./img/discovery_features_080322.png
[img Discovery Study page metadata]: ./img/discovery_study_page_datafiles.png
[img Discovery study page]: ./img/discovery_study_page.png
[img download notebook]: ./img/workspace_notebook_download_080422.png
[img Gen3 logo]: ./img/gen3blue.png
[img Jupyter logo]: ./img/workspace_jupyter_logo.png
[img Login other commons]: ./img/profile_login_other_commons.png
[img login]: ./img/brh-login.png
[img New Notebook]: ./img/workspace_new_080322.png
[img Notebook save]: ./img/workspace_notebook_save_080322.png
[img open data in wksp]: ./img/open_data_in_workspace.png
[img PD folder]: ./img/workspace_pd_folder_080422.png
[img profile]: ./img/profile_access.png
[img req access]: ./img/profile_login_other_commons.png
[img STR credit]: ./img/brh-portal-strides-credits.png
[img STR grant]: ./img/brh-portal-strides-grant.png
[img STRIDES payment]: ./img/brh-portal-options.png
[img Terminate workspace]: ./img/workspace_terminate_2.png
[img wksp register]: ./img/brh-portal-login-strides.png
[img Workspace access success]: ./img/workspace_access_success.png
[img Workspace Data Folder]: ./img/workspace_data_folder_080322.png
[img Workspace launch status]: ./img/workspace_launch.png
[img workspace manifest]: ./img/open_in_workspace_manifest_path.png
[img Workspace shutdown 2']: ./img/workspace_shutdown_sign_2.png
[img workspace upload]: ./img/workspace_upload_080322.png
[img Workspaces access request]: ./img/workspace_access_form.png
[img workspaces]: ./img/workspace_flavors_080322.png
[img Yes access]: ./img/access_YES.png
[img open Workspace AM]: ./img/open-wkspc-acct-mgr.png
[img Request persistent pay]: ./img/persistent-paymodel-request.png
[img Link to pay Portal]: ./img/link-to-pp.png
[img Pay Portal Profile]: ./img/payportal-profile.png
[img request BillingID]: ./img/request-billingid.png
[img Request Direct Pay workspace]: ./img/request-OCC-workspace.png

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
[Workspace timeout]: https://brh.data-commons.org/dashboard/Public/index.html#AutomaticWorkspaceShutdown
[Workspaces page]: 09-workspace_page.md
[BRH wksp access req form]: https://brh.data-commons.org/workspace/request-access
[Workspace Acct Mgr]: https://brh-portal.org/
<!-- markdown-link-check-disable -->
[Req new wksp]: https://brh-portal.org/request-workspace
<!-- markdown-link-check-enable -->
[OCC Payment Portal]: https://payments.occ-data.org/
[Payment Portal Profile]: https://payments.occ-data.org/profile/
[OCC Request BillingID]: https://payments.occ-data.org/request-billingid/
[OCC billing]: mailto:billing@occ-data.org
