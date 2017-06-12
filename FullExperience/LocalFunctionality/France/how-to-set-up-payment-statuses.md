---
title: "How to: Set Up Payment Statuses"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "payment management, statuses"
  - "payment status"
ms.assetid: b5808505-56e8-4989-ad36-9f7250df6c82
caps.latest.revision: 21
ms.author: "edupont"
manager: "terryaus"
translation.priority.ht: 
  - "fr-fr"
---
# How to: Set Up Payment Statuses
To use payment management, you must set up payment statuses to define payment document progress levels. You must define a set of statuses for each payment class. For more information, see [How to: Set Up Payment Classes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-payment-classes.md).  
  
### To set up payment statuses  
  
1.  In the **Setup** box, enter **Payment Slip Setup**, and then choose the relevant link.  
  
2.  Select a payment class, and then, on the **Home** tab, in the **Process** group, choose **Status**.  
  
3.  In the **Payment Status** window, on the **Home** tab, choose **New**.  
  
4.  Fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Name**|The payment status description.|  
    |**RIB**|Select to indicate that information about the Relevé d Identité Bancaire \(RIB\) statement for the customer or vendor must be displayed in the payment lines. The RIB information includes the bank branch number, agency code, bank account number, bank name, RIB key, and key verification.|  
    |**Look**|Select to indicate that the payment document lines that have reached this payment status can be edited and viewed in the **View\/Edit Payment Line** window.<br /><br /> For more information, see [View\-Edit Payment Line](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/-$-n_10862-view-edit-payment-line-$-.md).|  
    |**ReportMenu**|Select to indicate that the documents that have reached this payment status can be printed.|  
    |**Amount**|Select to display the amount in the payment lines.|  
    |**Payment in Progress**|Select to indicate that all billing and payment lines with this status must be considered when calculating the payments in progress.|  
    |**Archiving Authorized**|Select to indicate that payment headers with this payment status can be archived.|  
  
5.  Choose the **OK** button.  
  
## See Also  
 [View\-Edit Payment Line](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/-$-n_10862-view-edit-payment-line-$-.md)   
 [Payment Management](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/payment-management.md)   
 [How to: Set Up Payment Classes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-payment-classes.md)   
 [How to: Set Up Payment Steps](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-payment-steps.md)   
 [How to: Set Up Payment Addresses](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-set-up-payment-addresses.md)   
 [How to: Create Payment Slips](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-create-payment-slips.md)   
 [How to: Post Payment Slips](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-post-payment-slips.md)   
 [How to: Archive Payment Slips](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-archive-payment-slips.md)   
 [How to: Export or Import Payment Management Setup Parameters](../../LocalFunctionalityForMicrosoftDynamicsNav2016/France/how-to-export-or-import-payment-management-setup-parameters.md)