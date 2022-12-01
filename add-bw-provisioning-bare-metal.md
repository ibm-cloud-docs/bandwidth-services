---

copyright:
  years: 2022
lastupdated: "2022-11-30"

keywords: bandwidth services

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# Managing bare metal server bandwidth
 {: #how-to-add-and-upgrade-bare-metal-server-bw}

You can add bandwidth when you provision Bare Metal Servers for Classic. You can purchase larger allocations at a reduced cost compared to the overage rate.
{: shortdesc}

## Selecting bandwidth while provisioning bare metal servers
{: #how-to-add-bw-to-bare-metal}
{: ui}

To add bandwidth when you provision a bare metal server in the UI, follow these steps:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select **Catalog** from the menu bar on the header.
1. Select the **Bare Metal Servers for Classic** tile and provision your new virtual server instance. To learn more, see [Selecting from the most popular servers](/docs/bare-metal?topic=bare-metal-bm-select-popular-servers).
1. In the Network interface section, find the **Public egress - bandwidth** option. Then, select the amount of bandwidth that you want to add to your server's allocation. Bandwidth is offered in tiers.

   Public bandwidth usage over GB allocation is charged per GB. Also, public bandwidth egress (or bandwidth allocation) pricing depends on regions as indicated in **Pricing plans by region** on the [Bandwidth packages from IBM Cloud](https://www.ibm.com/cloud/bandwidth){: external} website.
   {: important}

![Bandwidth options while provisioning a bare metal server](images/bw-bare-metal-provisioning.svg "Bandwidth options while provisioning a bare metal server"){: caption="Figure 1. Bandwidth options while provisioning a bare metal server" caption-side="bottom"}

## Upgrading bandwidth on bare metal servers
{: #how-to-upgrade-bw-bare-metal}
{: ui}

To upgrade bandwidth on a bare metal server by using the UI, follow these steps:

1. From your browser, open the [{{site.data.keyword.cloud_notm}} console](/login){: external} and log in to your account.
1. Select the Navigation Menu ![Navigation Menu](../icons/icon_hamburger.svg), then click **Classic Infrastructure**.
1. Select **Devices > Device list**.
1. Click on the name of the bare metal server that you are modifying.
1. On the device's details page, find the VLAN Trunking section, then the Public bandwidth allocation section. Next to the Current billing cycle bandwidth allocation details, click **Modify**. 
1. Select a bandwidth upgrade option, then select if you want to update the device immediately or schedule the update for a later date and time. 
1. Add any notes, then click **Continue**. 

A 0 GB bandwidth allocation indicates a fully metered device, and an unspecified bandwidth allocation indicates a device with unlimited bandwidth. Both fully metered devices and devices with unlimited bandwidth are ineligible for bandwidth pooling.
{: note}

![Upgrading bandwidth on a bare metal server](images/upgrade-bw-bare-metal.svg "Upgrading bandwidth on a bare metal server"){: caption="Figure 2. Upgrading bandwidth on a bare metal server" caption-side="bottom"}
