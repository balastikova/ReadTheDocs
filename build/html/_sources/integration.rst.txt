Office 365 integration
======================

.. contents:: :local:

Safetica 9.5 brings automated and much simplified configuration of auditing and protection features for your e-mails and files stored in the cloud. Thanks to Office 365 integration, you will be able not only to audit cloud e-mails and files, but also to protect your e-mail using configured Safetica DLP policies. **WebSafetica service is required for this integration to work correctly**.

To be able to configure all the features mentioned below, you will need to log in to your Azure tenant with administrator rights so that Safetica is granted the necessary permissions. These permissions are only granted temporarily for the configuration of the needed settings.

*Note*: For now, Safetica can only connect to one tenant at a time. If you would like to switch to a different tenant, Safetica must perform a cleanup of settings. This might take a while, and you will only be able to connect to another tenant once the cleanup is finished.


Safetica Exchange Online audit and protection
------------------------------------------------
In Safetica, you can both audit your cloud e-mail and protect it using your DLP policies.

The auditing feature uses e-mail settings from Safetica Auditor to monitor files moving through the cloud. The DLP policy integration currently only supports general Safetica policies and policies applied to metadata-based data categories.

Safetica DLP policies are applied to matching Azure AD users (e.g. root DLP policy will be applied to all Azure AD users present in the Safetica user tree; a policy for a specific node will only be applied to  the Azure AD users belonging to this node etc.). DLP policies are applied to all Azure AD users, regardless of whether they have Safetica Client installed on their computers or not.

To enable auditing and/or Safetica DLP protection for your Exchange Online cloud e-mails:

#. Log in to **Safetica Management Console**.
#. Go to **Maintenance/Integration settings/Office 365 Integration**.
#. To enable the auditing feature, use the **Audit and log Office 365 e-mail** slider.
#. To enable Safetica DLP protection, use the **Apply Safetica DLP policies to Office 365 e-mail** slider.
#. Click [✔]. An Azure tenant sign-in window may appear.


Safetica OneDrive and SharePoint audit
----------------------------------------------
Safetica can also perform file monitoring for OneDrive and SharePoint, so you can see what files are downloaded or publicly shared. Audit logs, however, can currently only be viewed in **WebSafetica** under Data **Security/Office 365**.

To enable this feature:

#. Log in to **Safetica Management Console**.
#. Go to **Maintenance/Integration settings/Office 365 Integration**.
#. Enable this feature by using the **Audit and log Office 365 file operations** slider.
#. Click [✔]. An Azure tenant sign-in window may appear.

You can learn more about Office 365 integration in this introduction video:

.. raw:: html

    <iframe width="560" height="315" src="_static/O365_Integration.mp4" frameborder="0" allowfullscreen></iframe>