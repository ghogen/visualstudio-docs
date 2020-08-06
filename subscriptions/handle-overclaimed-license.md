---
title: Handle overallocated licenses | Microsoft Docs
author: evanwindom
ms.author: lank
manager: lank
ms.assetid: a747100c-6f08-41a4-aaad-05099741742b
ms.date: 03/03/2020
ms.topic: conceptual
description:  Learn how administrators can resolve over-allocated subscriptions
---

# Over-allocated subscriptions
Sometimes orders are changed after subscribers have been added, which can result in having more assigned subscriptions than licenses owned by your company. This is called "over-allocation".  

To see your subscripton allocations, click on the top icon at the left to open the allocations pane.  

> [!NOTE]
> Over-allocations are not allowed in Open License programs.  Also, other programs may display this information in the portal differently.
>
> [!div class="mx-imgBorder"]
> ![Notice of Over-claimed Subscriptions](_img/over-claimed/over-claimed-alert.png "The number of over-allocations is listed in the overview, and is represented by the hashed bar on the graph for each subscription type.")

Notice that the display uses a hashed bar to indicate over-allocated subscriptions.  The number of over-allocations across all subscription types is included in the Overview section at the top, and each subscription level also displays its own allocation status.  

## Resolve over-allocated subscriptions
There are several ways to resolve overallocations:
- Contact your reseller to purchase additional subscriptions.
- Wait until your annual true-up period and pay for the overallocated subscriptions at that point. 
- Delete some subscription assignments.  (This will not prevent the need for payment at the annual true-up as the true-up is based on the maximum number of subscriptions assigned at any time during the year.)

## Billing and true-up
If your organization has an Enterprise Agreement (EA), admins are able to assign subscriptions without purchasing them, and pay for them later through a reconciliation process known as a "true-up".  When you overallocate, your organization will be billed for the maximum number of subscriptions assigned to users during the "true-up".  This is true even if you no longer have the maximum number of subscriptions assigned at the time the true-up takes place.  To learn more about monitoring your maximum usage, visit the [Maximum Usage](maximum-usage.md) topic.

> [!Important]
> If Visual Studio Subscriptions with GitHub Enterprise are assigned by Visual Studio subscription admins and there has never been a purchase of those subscriptions, they will not be visible to GitHub Enterprise admins within the organization. To ensure GitHub Enterprise subscriptions are visible, a purchase including **at least one** Visual Studio Professional with GitHub Enterprise or Visual Studio Enterprise with GitHub Enterprise subscription should be made the first time the subscriptions are assigned.
>
> It is the customer’s responsibility to ensure that for each GitHub subscription that is assigned there is a corresponding Visual Studio with GitHub subscription assigned in the Manage portal to remain in compliance with the licensing requirements for this subscription.

## See also
- [Visual Studio documentation](https://docs.microsoft.com/visualstudio/)
- [Azure DevOps documentation](https://docs.microsoft.com/azure/devops/)
- [Azure documentation](https://docs.microsoft.com/azure/)
- [Microsoft 365 documentation](https://docs.microsoft.com/microsoft-365/)

## Next steps
- Learn more about managing [Visual Studio Subscriptions with GitHub Enterprise](assign-github.md).
- For assistance with sales, subscriptions, accounts and billing for Visual Studio Subscriptions, contact Visual Studio [Subscriptions Support](https://visualstudio.microsoft.com/subscriptions/support/).