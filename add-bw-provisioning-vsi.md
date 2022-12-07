---

copyright:
  years: 2022
lastupdated: "2022-12-07"

keywords: bandwidth services

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# Managing virtual server instance bandwidth
 {: #how-to-add-and-upgrade-vsi-bw}

You can add bandwidth when you provision virtual server instances. You can upgrade bandwidth by purchasing larger allocations at a reduced cost compared to the bandwidth overage rate.
{: shortdesc}

## Selecting bandwidth while provisioning virtual server instances
{: #how-to-add-bw-to-vsi}
{: ui}

To add bandwidth while provisioning a virtual server instance by using the UI, follow these steps:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select **Catalog** from the menu bar on the header. 
1. Select the **Virtual Server for Classic** tile and [provision your new virtual server instance](/docs/virtual-servers?topic=virtual-servers-ordering-vs-public).
1. In the Network interface section, find the **Public egress - bandwidth** option. Then, select the amount of bandwidth that you want to add to your server.
 
   Public bandwidth usage over GB allocation is charged per GB. Also, public bandwidth egress (or bandwidth allocation) pricing depends on regions as indicated in **Pricing plans by region** on the [Bandwidth packages from IBM Cloud](https://www.ibm.com/cloud/bandwidth){: external} website.
   {: important}

![Bandwidth options while provisioning a virtual server instance](images/bw-vsi-provisioning.svg "Bandwidth options while provisioning a virtual server instance"){: caption="Figure 1. Bandwidth options while provisioning a virtual server instance" caption-side="bottom"}

## Upgrading bandwidth on a virtual server instance
{: #how-to-upgrade-bw-vsi}
{: ui}

To upgrade bandwidth on a virtual server instance by using the UI, follow these steps:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select the Navigation menu ![Navigation menu](../icons/icon_hamburger.svg), then click **Classic Infrastructure**.
1. Select **Devices > Device list**.
1. Click the name of the virtual server instance that you are modifying.
1. On the device's details page, find the Network Details section, then the Public bandwidth allocation section. Beside the Current billing cycle bandwidth allocation details, click **Modify**. 
1. Select a bandwidth upgrade option, then select if you want to update the device immediately or schedule out the update for a later date and time. 
1. Add any notes, then click **Continue**. 

A 0 GB bandwidth allocation indicates a fully metered device, and an unspecified bandwidth allocation indicates a device with unlimited bandwidth. Both fully metered devices and devices with unlimited bandwidth are ineligible for bandwidth pools. 
{: note}

![Upgrading bandwidth on a virtual server instance](images/upgrade-bw-vsi.svg "Upgrading bandwidth on a virtual server instance"){: caption="Figure 2. Upgrading bandwidth on a virtual server instance" caption-side="bottom"}
