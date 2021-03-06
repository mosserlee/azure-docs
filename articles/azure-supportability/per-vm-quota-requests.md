---
title: Azure per VM vCPU quota increase requests | Microsoft Docs
description: per VM vCPU quota increase requests
author: sowmyavenkat86
ms.author: svenkat
ms.date: 06/07/2019
ms.topic: article
ms.service: azure-supportability
ms.assetid: ce37c848-ddd9-46ab-978e-6a1445728a3b

---

# Standard quota: per VM Series vCPU limit increase

Resource Manager supports two types of vCPU quotas for virtual machines. **Pay-as-you-go VMs and Reserved VM Instances** use standard quota. **Low priority VMs** use Low priority quota. 
Standard vCPU quota for pay-as-you-go and Reserved VM Instances is enforced at two tiers for each subscription in each region

The first tier is the **Total Regional vCPUs limit** (across all VM Series), and the second tier is the **per VM Series vCPUs limit** (such as the Dv3-series vCPUs). Anytime a new VM is to be deployed, the sum of new and existing vCPUs usage for that VM Series must not exceed the vCPU quota approved for that particular VM Series. Further, the total new and existing vCPU count deployed across all VM Series should not exceed the Total Regional vCPUs quota approved for the subscription. If either of those quotas are exceeded, the VM deployment will not be allowed.
You can request an increase of the vCPUs quota limit for the VM series from Azure portal. An increase in the VM Series quota automatically increases the Total Regional vCPUs limit by the same amount. 

Learn more about standard vCPU quotas on the [Virtual machine vCPU quotas page](https://docs.microsoft.com/azure/virtual-machines/windows/quotas) and [Azure subscription and service limits page](https://docs.microsoft.com/azure/azure-supportability/classic-deployment-model-quota-increase-requests). 

Learn more about increasing the regional vCPU limit for standard quota [here](https://docs.microsoft.com/azure/azure-supportability/regional-quota-requests). 

Learn more about **increasing Low priority VM vCPU limits** [here](https://docs.microsoft.com/azure/azure-supportability/low-priority-quota).

You can request an increase in **standard vCPU quota limits per VM Series** via **Help + Support** blade or the **Usages + Quota** blade in the portal.

## Request standard vCPU quota increase per VM Series at subscription level using the Help + Support blade

Follow the instructions below to create a support request via Azure's 'Help + Support' blade available in the Azure portal. 

You can also request Quota for multiple regions through a single support case. Refer to Step 11 below for details.

1. From https://portal.azure.com, select **Help + Support**.

   ![Help + Support](./media/resource-manager-core-quotas-request/helpsupport.png)
 
2.  Select **New support request**. 

     ![New support request](./media/resource-manager-core-quotas-request/newsupportrequest.png)

3. In the Issue type drop-down, choose **Service and subscription limits (quotas)**.

   ![Issue type drop-down](./media/resource-manager-core-quotas-request/issuetypedropdown.png)

4. Select the subscription that needs an increased quota.

   ![Select subscription newSR](./media/resource-manager-core-quotas-request/select-subscription-sr.png)
   
5. Select **Compute -VM (cores-vCPUs) subscription  limit increases** in **quota type** drop-down. 

   ![Select quota type](./media/resource-manager-core-quotas-request/select-quota-type.png)

6. In **Problem Details**, provide additional information to help process your request by clicking **Provide details**.

   ![Provide details](./media/resource-manager-core-quotas-request/provide-details.png)

7. In the **Quota details** panel, select **Deployment model** and select a **location.**

   ![Quota Details DM](./media/resource-manager-core-quotas-request/1-7.png)

8. For the selected location, select **Type** value as **‘Standard’**. You can request both Standard and Low priority quota types from a single support case through multi-selection support on the **Type** field. Learn more about **increasing Low priority quota limits** on the **<> page**.

   ![SKU Family](./media/resource-manager-core-quotas-request/1-8.png)

9. Select the **SKU families** that require an increase

   ![SKU Family](./media/resource-manager-core-quotas-request/1-9.png)

10. Enter the new limits you would like on the subscription. To remove a line, uncheck the SKU from the SKU family drop-down or click the discard "x" icon. 

   ![New Limits](./media/resource-manager-core-quotas-request/1-10.png)

11. To request Quota for more than one location you can check on another **location** from the drop-down and select appropriate VM Type. This step preloads SKU families selected for earlier **location** against the new location and you can simply enter the new limits you would like.

   ![Multiple locations](./media/resource-manager-core-quotas-request/1-11.png)
   
12. After entering the desired quota for each SKU family, click **Save and Continue** on the Quota details panel to continue with the support request creation.

## Request standard vCPU quota increase per VM Series at subscription level using Usages + Quota blade

Follow the instructions below using to create a support request via Azure's 'Usage + quota' blade available in the Azure portal.

You can also **request Quota for multiple regions** through a single support case. Refer to Step 10 below for details

1. From https://portal.azure.com, select **Subscriptions**.

   ![Subscriptions](./media/resource-manager-core-quotas-request/subscriptions.png)

2. Select the subscription that needs an increased quota.

   ![Select subscription](./media/resource-manager-core-quotas-request/select-subscription.png)

3. Select **Usage + quotas**

   ![Select usage and quotas](./media/resource-manager-core-quotas-request/select-usage-quotas.png)

4. In the upper right corner, select **Request increase**.

   ![Request increase](./media/resource-manager-core-quotas-request/request-increase.png)

5. Select **Compute-VM (cores-vCPUs) subscription limit increases** as the quote type. 

   ![Fill in form](./media/resource-manager-core-quotas-request/select-quota-type.png)
   
6. In the **Quota details** panel, select Deployment model and select a location.

   ![Quota Problem blade](./media/resource-manager-core-quotas-request/1-1-6.png)

7. For the selected location, select **Type** value as **‘Standard’**. You can request both Standard and Low Priority quota types from a single support case through multi-selection support on the **Type** field. Learn more about **increasing Low Priority vCPUs limits** on this [page](https://docs.microsoft.com/azure/azure-supportability/low-priority-quota).

   ![SKU series selected](./media/resource-manager-core-quotas-request/1-1-7.png)
   
   
8. Select the **SKU Families** that require an increase

   ![SKU series selected](./media/resource-manager-core-quotas-request/1-1-8.png)

9. Enter the new limits you would like on the subscription. To remove a line, uncheck the SKU from the SKU family drop-down or click the discard "x" icon. 

   ![SKU new quota request](./media/resource-manager-core-quotas-request/1-1-9.png)
   

10. To request Quota for more than one location you can check on another **location** from the drop-down and select appropriate VM Type. This step preloads SKU families selected for earlier **location** against the new location and you can simply enter the new limits you would like.
   
    ![SKU new quota request](./media/resource-manager-core-quotas-request/1-1-10.png)
 
