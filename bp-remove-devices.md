---

copyright:
  years: 2022
lastupdated: "2022-12-07"

keywords: bandwidth services, bandwidth pools

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# Removing devices from bandwidth pools
{: #how-to-remove-devices-from-bw-pools}
{: ui}

To remove devices from a bandwidth pool by using the UI, follow these steps:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select the Navigation menu ![Navigation menu](../icons/icon_hamburger.svg), then click **Classic Infrastructure**.
1. Select **Network > Bandwidth > Pools**.
1. Locate the bandwidth pool that contains the device that you want to remove. Use the **Region** and **Overage status** filters as necessary.
1. Click the name of the device to access the bandwidth pool's details page. 
1. In the **Name** column of the devices list table, select the checkboxes next to the devices that you want to remove from the pool. 
1. Click **Remove**. 
1. In the side section that appears, acknowledge that you understand that the device remains active in the pool until the next billing date. Review the summary of billing changes and the new monthly cost of your pool.
1. Click **Remove**. 

   The device remains active in your pool and continues to meter until it is permanently removed at the end of your billing cycle. 
   {: note}

1. Select **Scheduled** status in the **Removal** column in your bandwidth pool's device table to check the scheduled removal date of the device, or to unschedule the device's removal from the pool. For more information, see [Unscheduling device removal from bandwidth pools](/docs/bandwidth-pools?topic=bandwidth-pools-how-to-unschedule-device-removal-from-bw-pools).

![Remove a device from a bandwidth pool](images/bw-remove-device-from-pool.svg "Remove a device from a bandwidth pool"){: caption="Figure 1. Remove a device from a bandwidth pool" caption-side="bottom"}
