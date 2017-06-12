---
title: "Collect Payments with SEPA Direct Debit"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
ms.assetid: 376fa7a0-4f5d-4a1d-8356-24171d76cd68
caps.latest.revision: 8
ms.author: "sgroespe"
translation.priority.ht: 
  - "da-dk"
  - "de-at"
  - "de-ch"
  - "de-de"
  - "en-au"
  - "en-ca"
  - "en-gb"
  - "en-in"
  - "en-nz"
  - "es-es"
  - "es-mx"
  - "fi-fi"
  - "fr-be"
  - "fr-ca"
  - "fr-ch"
  - "fr-fr"
  - "is-is"
  - "it-ch"
  - "it-it"
  - "nb-no"
  - "nl-be"
  - "nl-nl"
  - "ru-ru"
  - "sv-se"
---
# Collect Payments with SEPA Direct Debit
With your customer’s consent, you can collect payments directly from the customer’s bank account according to the SEPA format.  
  
 First, set up the export format of the bank file that instructs your bank to perform a direct debit. Then, set up the customer’s payment method. Last, set up the direct\-debit mandate that reflects your agreement with the customer to collect their payments in a certain agreement period.  
  
 To instruct the bank to transfer the payment amount from the customer’s bank account to your company’s account, you create a direct\-debit collection entry, which holds information about bank accounts, the affected sales invoices, and the direct\-debit mandate. You then export an XML file that is based on the collection entry, which you send to your bank for processing. Any payments that could not be processed will be communicated to you by your bank, and you must then manually reject the direct debit\-collection entries in question.  
  
 You can set up standard customer sales codes with the direct\-debit payment method and mandate information. You can then use the **Create Standard Cust. Invoices** batch job to generate multiple sales invoices with the direct\-debit information prefilled. This is can be done manually or automatically, according to the payment due date.  
  
 When payments are successfully processed, as communicated by your bank, you can post the payment receipts either directly from the **Direct Debit Collect. Entries** window or by moving the payment lines to the journal where you post payment receipts, such as the **Cash Receipt Journal** window. Alternatively, depending on your cash management process, you can wait and just apply the payments as a part of bank reconciliation. For more information, see [How to: Match Bank Statement Lines with Bank Account Ledger Entries](../Finance/how-to-match-bank-statement-lines-with-bank-account-ledger-entries.md).  
  
> [!NOTE]  
>  To collect payments using SEPA Direct Debit, the currency on the sales invoice must be EURO.  
  
 The following table describes a sequence of tasks, with links to the topics that describe them. These tasks are listed in the order in which they are generally performed.  
  
|**To**|**See**|  
|------------|-------------|  
|Prepare bank account formats, payment methods, and customer agreements for SEPA direct debit.|[How to: Set Up SEPA Direct Debit](../BusinessFunctionality/DataExchange/how-to-set-up-sepa-direct-debit.md)|  
|Instruct your bank to transfer payment amounts from your customers’ bank accounts to your company’s account according to your setup of SEPA direct debit.|[How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File](../BusinessFunctionality/DataExchange/how-to-create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file.md)|  
|Set up standard customer sales codes for direct\-debit invoices and generate sales invoices with direct\-debit information when the invoices are due for payment.|[How to: Create Multiple Sales Invoices Based on Standard Sales Codes](../Finance/how-to-create-multiple-sales-invoices-based-on-standard-sales-codes.md)|  
|Post payments made as SEPA direct debits.|[How to: Post SEPA Direct Debit Payment Receipts](../Finance/how-to-post-sepa-direct-debit-payment-receipts.md)|  
  
## See Also  
 [Direct Debit Collect. Entries](../Topic/\($%20N_1208%20Direct%20Debit%20Collect.%20Entries%20$\).md)   
 [Direct Debit Collect. Entries](../Topic/\($%20N_1208%20Direct%20Debit%20Collect.%20Entries%20$\).md)   
 [Create Recurring Sales Inv.](../Topic/\($%20R_172%20Create%20Recurring%20Sales%20Inv.%20$\).md)   
 [Manage Receivables](../Finance/manage-receivables.md)