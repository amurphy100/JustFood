---
title: "How to: Fill In the Revaluation Journal with the Batch Job"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "journals, revaluation"
  - "revaluing inventory, batch jobs"
  - "inventory, revaluation"
ms.assetid: 264224ef-93f1-43c7-ae68-b6abc64bbd90
caps.latest.revision: 5
ms.author: "sgroespe"
manager: "terryaus"
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
# How to: Fill In the Revaluation Journal with the Batch Job
If you want to appreciate or depreciate an item or a specific item ledger entry, you must use the revaluation journal.  
  
 First, you must fill in the revaluation journal with information about the current, calculated value of the specified item or item ledger entry. You can do this [manually](../DesignAndEngineering/how-to-fill-in-revaluation-journals-manually.md) or use the **Calculate Inventory Value** batch job.  
  
### To fill in the revaluation journal with the batch job  
  
1.  In the **Search** box, enter **Revaluation Journal**, and then choose the related link.  
  
2.  As the calculation of inventory value can be rather time consuming, it is not desirable if the calculation is cancelled because of a precondition not met. Therefore, the **Calculate Inventory Value \- Test** batch job can be used. This test report checks preconditions for the inventory value calculation.  
  
3.  On the **Actions** tab, in the **Functions** group, choose **Calculate Inventory Value**. The **Calculate Inventory Value** window opens.  
  
4.  On the **Item** FastTab, set a filter if you want to select a specific item number or select an item from a specific location or a specific variant of an item.  
  
5.  In the remaining fields, specify the conditions to use to create the journal lines.  
  
6.  Choose the **OK** button.  
  
 You can now revalue the selected item ledger entries. When you have filled in the revaluation journal, you can post the journal.  
  
 The value entries are created to reflect the revaluing. You can see these from the item card.  
  
## See Also  
 [Inventory Revaluation](../DesignAndEngineering/inventory-revaluation.md)   
 [How to: Enter New Values When Revaluing Items](../DesignAndEngineering/how-to-enter-new-values-when-revaluing-items.md)   
 [How to: Fill In Revaluation Journals Manually](../DesignAndEngineering/how-to-fill-in-revaluation-journals-manually.md)