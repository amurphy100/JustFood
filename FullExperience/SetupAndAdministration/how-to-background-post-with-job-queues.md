---
title: "How to: Background Post with Job Queues"
ms.custom: na
ms.date: "03-03-2017"
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: "article"
helpviewer_keywords: 
  - "posting, background"
  - "job queues, background posting"
ms.assetid: 9d9432e7-ed67-419a-9b14-fcea15cb48cb
caps.latest.revision: 12
ms.author: "edupont"
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
# How to: Background Post with Job Queues
Job queues are an effective tool to schedule the running of business processes in the background. For example, there may be an instance in which multiple users are trying to post sales orders at the same time, but only one order can be processed at a time. By setting up a background posting routine, you can place the postings in a queue for processing in the background.  
  
 Alternatively, you may want to schedule postings for hours when it is convenient for your organization. For example, it may make sense in your business to run certain routines when most of the data entry for the day has concluded. You can achieve this by setting the job queue up to run various batch post reports, such as the **Batch Post Sales Orders**, **Batch Post Sales Invoices**, and **Batch Post Sales Credit Memos** reports.  
  
 [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] supports background posting for the following document types:  
  
-   Sales: sales order, return order, credit memo, invoice  
  
-   Purchases: purchase order, return order, credit memo, invoice  
  
 If the job queue cannot post the sales order, the status is changed to **Error**, and the sales order is added to the list of sales orders that the user will have to handle.  
  
> [!NOTE]  
>  When you schedule a document for posting and the posting process begins, the posting routine is automatically configured to time out within two hours if the posting routine stops responding for any reason.  
  
 The following procedure demonstrates how to use a job queue to do background posting of sales orders.  
  
### To post in the background using a job queue  
  
1.  In the **Search** box, enter **Sales & Receivables Setup**, and then choose the related link.  
  
2.  In the **Sales & Receivables Setup** window, expand the **Background Posting** FastTab.  
  
3.  Select the **Post Documents via Job Queue** check box.  
  
4.  To filter to the sales order type of job queue entry, choose the **Job Queue Category Code** field, and select the **SalesPost** category. When you choose this category, you are filtering to all sales orders that match any job queue that has the same category code.  
  
     [!INCLUDE[navnow](../ApplicationDesign/includes/navnow_md.md)] creates a job queue entry that specifies codeunit 88. The creation of the entry is automatic. For more information about how to create a job queue entry, see [Use Job Queues to Schedule Tasks](../SetupAndAdministration/use-job-queues-to-schedule-tasks.md).  
  
5.  In the **Search** box, enter **Job Queues**, and then choose the related link. For more information, see [How to: Set Up Job Queues](../SetupAndAdministration/how-to-set-up-job-queues.md).  
  
6.  In the **Code** field, select the job queue code **SPPOST**, and on the **Home** tab, choose **Edit**.  
  
7.  Expand the **NAS Settings** FastTab, and clear the **Start Automatically from NAS** check box. For more information on starting job queues, see [How to: Set Up Job Queues](../SetupAndAdministration/how-to-set-up-job-queues.md).  
  
8.  On the **Home** tab, in the **Process** group, choose **Start Job Queue**.  
  
9. To verify that the job queue is working as expected, post a sales order. For more information, see [How to: Post Sales Orders](../Sales/how-to-post-sales-orders.md).  
  
    > [!TIP]  
    >  If you do not want to post an individual sales order that is scheduled for posting, you can remove it from the job queue.  
    >   
    >  1.  For the sales order page or the sales order list, customize the ribbon to add the following action: **Remove From Job Queue**. For more information, see [How to: Customize Ribbons](../SetupAndAdministration/how-to-customize-ribbons.md).  
    > 2.  Select the order that you want to remove from the queue, and in the group where you have added the action, choose **Remove From Job Queue**.  
  
10. In the **Search** box, enter **Job Queue Log Entries**, and then choose the related link.  
  
     In the **Job Queue Log Entries** window, you can see whether the sales order posting is in process or has succeeded in the job queue.  
  
 An alternative way to see your log entries is to use the **My Job Queue** part. For more information, see [How to: Use My Job Queue Part](../SetupAndAdministration/how-to-use-my-job-queue-part.md).  
  
 The next procedure explains the steps you need to take to post and print in the background.  
  
### To post and print in the background  
  
1.  Set up a printer to work in the background. For more information, see [How to: Specify Printer Selection for Reports](../WorkingWithDynamics/how-to-specify-printer-selection-for-reports.md) and [Printing Reports from a Background Session](../Topic/Printing%20Reports%20from%20a%20Background%20Session.md).  
  
2.  In the **Search** box, enter **Sales & Receivables Setup**, and then choose the related link.  
  
3.  In the **Sales & Receivables Setup** window, expand the **Background Posting** FastTab.  
  
4.  Select the **Post & Print with Job Queue** check box.  
  
5.  Follow the remaining steps in the rest of the preceding procedure to complete the task.  
  
> [!IMPORTANT]  
>  When you send a document to a printer, and the printer displays a dialog box, such as a request for credentials or a warning about low printer ink, your document is posted but not printed. The corresponding job queue entry eventually times out and the **Status** field is set to **Error**. Accordingly, we recommend that you do not use a printer setup that requires interaction with the display of printer dialog boxes in conjunction with background posting.  
  
## See Also  
 [How to: Set Up Job Queues](../SetupAndAdministration/how-to-set-up-job-queues.md)   
 [How to: Use My Job Queue Part](../SetupAndAdministration/how-to-use-my-job-queue-part.md)   
 [My Job Queue](../Topic/\($%20N_675%20My%20Job%20Queue%20$\).md)   
 [Printing Reports from a Background Session](../Topic/Printing%20Reports%20from%20a%20Background%20Session.md)