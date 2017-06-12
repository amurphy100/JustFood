---
title: "How to: Set Up Payment Line Information"
ms.custom: na
ms.date: "06-05-2016"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "remittance, payment lines"
  - "payment journals, remittance"
ms.assetid: 237b0715-6965-4972-8649-893bbf9f1f0e
caps.latest.revision: 3
ms.author: "edupont"
translation.priority.ht: 
  - "nb-no"
---
# How to: Set Up Payment Line Information
Payment journal line information for the remittance payment is set up in the **Payment Info** window.  
  
### To set up payment line information  
  
1.  In the **Search** box, enter **Payment Journals**, and then choose the related link.  
  
2.  On the **Navigate** tab, choose **Payment Info**.  
  
3.  In the **Payment Info** window, on the **General** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Remittance Account Code**|Select the remittance account code.|  
    |**15000018 Remittance Agreement Code**|Specify the agreement code assigned to the account code.|  
    |**Remittance Type**|Specify the remittance type assigned to the account code. Remittance types include **Domestic** and **Foreign**.|  
  
4.  On the **Domestic** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Recipient Ref. 1 – 3**|Specify the payment text which is sent to the vendor.|  
    |**KID \(Cust. id number\)**|Specify the number sent to the vendor during payment.|  
    |**Our Account. No.**|Specify the account number for your company.|  
    |**External Document No.**|Specify the number of the external document.|  
    |**Payment Type Code Domestic**|Specify the payment type code that is assigned to the payment.|  
  
    > [!NOTE]  
    >  The recipient reference and the KID number cannot be entered for the same payment. If the KID is used, this is the only information that the vendor receives.  
  
5.  On the **Foreign** FastTab, fill in the fields as described in the following table.  
  
    |[!INCLUDE[bp_tablefield](../../ApplicationDesign/includes/bp_tablefield_md.md)]|[!INCLUDE[bp_tabledescription](../../ApplicationDesign/includes/bp_tabledescription_md.md)]|  
    |---------------------------------|---------------------------------------|  
    |**Recipient Ref. Abroad**|Specify the payment text that is sent to the vendor.|  
    |**Payment Type Code Abroad**|Specify the payment type code that is assigned to the payment.|  
    |**Check**|Specify whether a check must be issued.<br /><br /> \* <br />                        **No** \- No check is issued.<br /><br /> \* **Send to employer** \- Check is issued and sent to the employer.<br /><br /> \* **Send to beneficiary** \- Check is issued and sent to the beneficiary.|  
    |**Urgent**|Select if the payment is urgent and should be treated as an urgent transfer.|  
    |**Agreed Exch. Rate**|Specify the exchange rate which the bank agrees upon.|  
    |**Agreed With**|Specify who the agreement is entered with, if an exchange rate is agreed upon.|  
    |**Futures Contract No.**|Specify the future contract number that is used for this payment.|  
    |**Futures Contract Exch. Rate**|Specify the future contract exchange rate that is used for this payment.|  
  
6.  Choose the **OK** button.  
  
## See Also  
 [Electronic Payments to Vendors in Norway](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/electronic-payments-to-vendors-in-norway.md)   
 [How to: Set Up Remittance Agreements](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-set-up-remittance-agreements.md)   
 [How to: Create Remittance Accounts](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-create-remittance-accounts.md)   
 [How to: Set Up Vendors for Remittance](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-set-up-vendors-for-remittance.md)   
 [Recipient Reference Codes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/recipient-reference-codes.md)   
 [How to: Create Remittance Suggestions](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-create-remittance-suggestions.md)   
 [How to: Create Manual Remittance Payments](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-create-manual-remittance-payments.md)   
 [How to: Test Remittance Payments](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-test-remittance-payments.md)   
 [How to: Export Remittance Payments](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-export-remittance-payments.md)   
 [Types of Payment Returns Files](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/types-of-payment-returns-files.md)   
 [How to: Import Payment Return Data](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-import-payment-return-data.md)   
 [How to: Delete Remittance Payment Orders](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-delete-remittance-payment-orders.md)   
 [Remittance Errors](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/remittance-errors.md)   
 [How to: View Remittance Error Codes](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-view-remittance-error-codes.md)   
 [How to: Cancel Payments](../../LocalFunctionalityForMicrosoftDynamicsNav2016/Norway/how-to-cancel-payments.md)