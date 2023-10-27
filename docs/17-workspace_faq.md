# **Workspace FAQs**

## Workspace Questions (any funding source)

#### What happens if my trial access or funding runs out?

> When you have used all of your allotted time (trial access) or funding (persistent pay models), you will no longer be able to launch a workspace. You will not have access to your /pd folder. You will still be able to open the [BRH Workspace page][BRH Workspace], and log in to the [Workspace Account Manager][Workspace Acct Mgr]. You can request new account funding from the [Workspace Account Manager][Workspace Acct Mgr].

#### Is the persistent directory (/pd) shared among all the pay model options? Will my data be available in all my workspace accounts?

> No. Currently, the /pd folder is separate for each workspace pay model account. So, the data from your /pd for your trial access account will not automatically be available in the /pd for your Direct Pay workspace account or your STRIDES workspace account.

#### How should I cite research done in BRH workspace?

> Make sure to cite the author of the data used in your research, the repository housing the data, and the BRH platform enabling your access to the data. [See details here][Cite BRH].

## Direct Pay workspace, Payment Portal, & BillingID questions

#### Why does my Hard Limit not match the amount of funding I purchased?

> As described in your Direct Pay User Agreement, some amount of your purchase is set aside for use for account operational expenses beyond compute costs. If you have further questions about this, please contact [billing@occ-data.org][OCC billing]

#### Can I get a refund on any unused compute funding I purchased?
> Unfortunately, as described in your Direct Pay User Agreement, OCC cannot offer refunds for unused compute time already purchased.

#### I've been using my workspace all day, but my total usage number hasn't changed at all.

> Data usage is monitored by AWS, and AWS makes updates several times a day. This means that you can possibly use the workspace for a number of hours before the compute usage is updated. Also, the update is sometimes delayed -- that is, a usage update from AWS could still be omitting usage in the hours preceding it.

#### What if I don't pay the renewal invoice before my usage exceeds the Hard Limit?

> If you do not pay the renewal invoice before you reach the Hard Limit, you will lose access to the Direct Pay account /pd, and you will be unable to launch any workspaces from the Direct Pay account. If you still have not renewed funding 2 months (60 days) after reaching your Hard Limit, we may delete the contents of the /pd for that account.

#### Why is the OCC Payment Portal a separate account?

> The OCC payment portal is for our third-party AWS reseller, the Open Commons Consortium (OCC). The site is [payments.occ-data.org][OCC Payment Portal]. This is a separate site and account because we want to protect your financial information; the OCC payment portal site follows more rigorous financial best practices. Please note that neither this site nor OCC as an organization will hold any of your payment information; when you pay an invoice, the actual payment information will go through a separate secure payment processor and is not stored anywhere after the charge is processed.

#### Can I change my email address associated with my OCC Payment Portal account?

> No. Unfortunately, you cannot change the email address associated with your BillingID or OCC Payment Portal account. You can create a new OCC Payment Portal account with another email address, but you will need to request a new BillingID for that account.

#### I didn’t receive my token for the Payment Portal login.

> It may take a couple minutes to send, but not more than that. Check your spam folder. If you don't see it there, you can request another token by clicking the Request Token button again.

#### My token for the OCC Payment Portal expired

> You can request another token by clicking Request Token again.

#### How can I find the terms for the Direct Pay billing agreement?

> When that document is available, it will be posted on the OCC Direct Pay site. We will link to it when available.

#### At what point am I actually paying for workspace funds - what step does the actual charge take place?

> You designate how much you want to purchase when you initially request your BillingID on the OCC Payment Portal. However, the invoice for this amount is not actually sent until after you have done both of the following:

1. receive a BillingID on the OCC Payment Portal
2. use this BillingID to request a Direct-Pay-funded workspace account in the Workspace Account Manager

> Once you have completed both of these, you will be sent an invoice - when you pay this invoice is when you submit your credit card number and actually pay the charged amount.

#### What credit cards can be used to pay for Direct Pay?

> We accept all major credit cards, including Visa, MasterCard, Discover, and American Express.
>
> We also accept ACH electronic payments from a bank account, Apple Pay, PayPal, and Venmo.

#### What are the different websites involved in purchasing and using Direct Pay for workspaces?

> **BRH Platform:** This is the main BRH site, with all the BRH data and the Workspace page. The site is [brh.data-commons.org][BRH Platform], and you can reach the [Workspace page][BRH Workspace] by clicking on the Workspace button at the top of the portal.
>
> **BRH Workspace Account Manager:** This is where you can request or view details of your Workspace accounts funded with persistent pay models. The site is [brh-portal.org][Workspace Acct Mgr], and you can also reach this site from the [BRH Workspace page][BRH Workspace] by clicking on the `Workspace Account Manager` link at the top left corner, in the Account Information section. This page will be built into the BRH Platform Workspace page in a future update (*i.e.*, it won't be a separate page).
>
> **OCC Payment Portal:** This is the payment portal site for our third-party AWS reseller, the Open Commons Consortium (OCC). Here, you can request a BillingID, specify the amount of Direct Pay funding you will want on your Direct Pay account, and track the status of your BillingID request. The site is [payments.occ-data.org][OCC Payment Portal]. *Note:* Neither this site nor OCC will hold any of your payment information; when you pay an invoice, the actual payment information will go through a separate secure payment processor and is not stored anywhere after the charge is processed.

## STRIDES Questions

#### What is the STRIDES Program?

> The NIH STRIDES Initiative is a program to help NIH-funded researchers accelerate biomedical research by reducing barriers to utilizing for-fee cloud services, like the BRH Workspace.

> The STRIDES program gives cost discounts and a host of other benefits to researchers with NIH grants and contracts.

#### What are the benefits for using the STRIDES program?

> STRIDES program benefits include:
>
> * Cost discounts on AWS services (e.g., compute, storage, and egress fees)
> * Premium-level [AWS Enterprise Support][AWS Enterprise Support]
> * [Training and education programs][STRIDES training]
> * and more! See the [STRIDES program benefits][STRIDES benefits] page for more information

#### Who is eligible for using the STRIDES program?

> Anyone with any NIH funding, for any NIH award type, is eligible for the benefits of the STRIDES Initiative.

#### What is the difference between STRIDES Credit and STRIDES Grant/Award Funded?

> The main difference is who is responsible for paying to provision the Workspace account.
>
> **STRIDES Grant/Award Funded:** This is the most common STRIDES account model. Here, the Workspace account is provisioned by organization receiving the NIH grant funds (generally a PI's institution). Researchers who have received NIH funding (e.g. a grant, contract, cooperative agreement, or other transaction agreement) can use these funds for the BRH workspace account. With this option, the researchers' organization will be responsible for payment.
>
> **STRIDES Credits** This is less common. Here, the payment for provisioning the Workspace account is made directly by NIH. Generally this is discussed with NIH ahead of submitting the request. With this option, once the request is approved, a new account with a set spending limit of will be provisioned by NIH directly for usage.


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
[BRH Workspace]: https://brh.data-commons.org/workspace
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
[Cite BRH]: https://uc-cdis.github.io/platform-citation/brh-cite/
[Workspace Acct Mgr]: https://brh-portal.org/
[Register for workspaces]: 05-workspace_registration.md
[Request study access]: 07-how_to_check_request_access.md
[STRIDES]: https://datascience.nih.gov/strides
[Workspace timeout]: https://brh.data-commons.org/dashboard/Public/index.html#AutomaticWorkspaceShutdown
[Workspaces page]: 09-workspace_page.md
[BRH wksp access req form]: https://brh.data-commons.org/workspace/request-access
[Req new wksp]: https://brh-portal.org/request-workspace
[OCC Payment Portal]: https://payments.occ-data.org/
[Payment Portal Profile]: https://payments.occ-data.org/profile/
[OCC Request BillingID]: https://payments.occ-data.org/request-billingid/
[STRIDES benefits]: https://cloud.nih.gov/about-strides/benefits/
[AWS Enterprise Support]: https://aws.amazon.com/premiumsupport/plans/enterprise/
[STRIDES training]: https://cloud.nih.gov/training/
[OCC billing]: mailto:billing@occ-data.org
