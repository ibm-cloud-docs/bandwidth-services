---

copyright:
  years: 2022
lastupdated: "2022-11-30"

keywords: bandwidth services, bandwidth pools

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# Adding devices to bandwidth pools 
{: #how-to-add-devices-to-ibm-cloud-bandwidth-pools}
{: ui}

If you want to add devices to a bandwidth pool, follow these steps by using the UI:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select the Navigation Menu ![Navigation Menu](../icons/icon_hamburger.svg), then click **Classic Infrastructure**.
1. Select **Network > Bandwidth > Summary**.
1. Locate the device that you want to add to a bandwidth pool. Use the **Location** and **Pool** filters as necessary.
   Each device that you add to a bandwidth pool incurs a cost to the pool. For more information, see [FAQs for bandwidth services](/docs/bandwidth-services?topic=bandwidth-services-faqs).
   {: note}
1. Under the **Pool** column of the device table, select **Add to pool**.
   Devices that are billed hourly (fully metered) and devices with unlimited allocation are not eligible for bandwidth pooling. 
   {: note}
1. In the **Add device to a Bandwidth pool** page, view the list of eligible pools.
1. Select an eligible bandwidth pool to add your device to that pool. 
1. In the **Summary** panel:
    - Review the cost of adding your devices to the pool.
    - Agree to the Terms and Conditions.
    - Click **Add devices to pool**.

Alternatively, you can access the bandwidth pool's details page to add devices. On the upper right of the device list, click **Add** and select eligible devices to add to your pool.
{: note}

![Bandwidth summary page](images/bw-summary-page.svg "Bandwidth summary page"){: caption="Figure 1. Bandwidth summary page" caption-side="bottom"}
