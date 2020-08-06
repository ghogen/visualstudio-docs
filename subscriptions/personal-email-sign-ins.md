---
title: Personal emails displayed in VLSC
author: evanwindom
ms.author: lank
manager: lank
ms.assetid: 3f4b0528-03f0-4a02-b3c3-a39292a9bbe1
ms.date: 04/10/2020
ms.topic: conceptual
description:  Visual Studio Subscriptions – Why Am I Seeing Hotmail or Gmail Addresses for My Subscribers?
---

# Visual Studio subscriptions – Why do I see personal accounts for my subscribers?
After companies migrated from the Volume Licensing Service Center (VLSC) to the new Visual Studio [Subscriptions Administration Portal](https://manage.visualstudio.com), administrators were surprised to find that the “Sign-in Email Address” for some subscribers shows a personal email address like Hotmail or Outlook.  

## Cause
This scenario occurs due to sign-in processes that were associated with the legacy MSDN subscriber experience. Users were migrated from the Volume License Service Center (VLSC) to the Visual Studio Subscriptions Administration Portal without modifications. Administrators may not have been aware that users had been using personal accounts to access their subscription benefits. Prior to the Visual Studio subscriber migrations, which were completed in 2016, there were two actions required to successfully use a Visual Studio Subscription:
1. The administrator “assigned” the subscription to an individual subscriber, using their work or school email address.
2. The subscriber “activated” the subscription.

During the subscriber activation process:
A Microsoft Account (MSA) was required to sign-in. If the subscriber didn’t attempt to make their work or school account (e.g. tasha@contoso.com) an MSA, they could create a new MSA or leverage an existing one. This resulted in their “Sign-in Email Address” being different than their “Assigned to Email Address”.

> [!NOTE]
> The modern subscriber experience on [https://my.visualstudio.com](https://my.visualstudio.com?wt.mc_id=o~msft~docs) supports both Work/School and Microsoft Account (MSA) identity types.

## Solution

> [!VIDEO https://www.microsoft.com/videoplayer/embed/RE4th6B]

To correct the problem, simply select the **Connect Emails** button and the system will attempt to match the accounts with MSAs to existing users in your organization’s Azure Active Directory (Azure AD) based on matching the first and last name. If there is an error, you can remove any match by clicking on the **X** to the right of the match.  

> [!div class="mx-imgBorder"]
> ![Connect Emails Button](_img/connect-emails/connect-emails-button.png)

You can also use the **Search Directory** to correct the errors or fill in missing information from your Azure AD. If the all the matches look correct, you can choose to “Select all matching subscribers”, rather than selecting them one at a time.  

> [!div class="mx-imgBorder"]
> ![Connect Emails Fly-out](_img/connect-emails/connect-emails-flyout.png)

Next click on “continue” which will take you to a screen outlining the changes to take place. If you agree, click “save” and the changes will be made. Your subscriber will also get a message informing them of the change the next time they sign in to their subscription.   

> [!div class="mx-imgBorder"]
> ![Connect Emails Confirmation](_img/connect-emails/connect-emails-confirm.png) 

> [!NOTE]
> When you edit the sign in email address this only updates the email used by the subscriber to sign in to their subscription on https://my.visualstudio.com. If the subscriber has already activated benefits such as Azure or Pluralsight using the other email address, they will need to continue to use those email addresses to access them. For any new benefits that they access, they should use the new email address. 

## See also
- [Visual Studio documentation](https://docs.microsoft.com/visualstudio/)
- [Azure DevOps documentation](https://docs.microsoft.com/azure/devops/)
- [Azure documentation](https://docs.microsoft.com/azure/)
- [Microsoft 365 documentation](https://docs.microsoft.com/microsoft-365/)

##  Next steps
- If you have updated the subscriber(s) email address(es), you may want to notify them that their sign-in information has changed.  They will also receive an email with the updated information.
- It may be useful to [filter the list of subscribers](search-license.md) in your organization to look for any sign in email addresses that may need to be changed.  
