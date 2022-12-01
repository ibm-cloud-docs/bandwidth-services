---

copyright:
  years: 2022
lastupdated: "2022-11-30"

keywords: bandwidth services, bandwidth pools

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# About bandwidth services
{: #about-bandwidth-services}

To reduce your overall bandwidth costs, it's important to consider your bandwidth service options. You can purchase and manage bandwidth for classic services in two ways, through metering on individual devices, or through collective-metering when you add a device to a bandwidth pool. 
{: shortdesc}

All inbound and outbound bandwidth inside the IBM Cloud Classic infrastructure is unlimited and cost-free for your servers' use. Public egress bandwidth is charged on a tiered basis, with a set allocation for each month of your servers' use.
 
Bandwidth usage is measured as egress traffic on a device's public interfaces.
{: note}

Bandwidth allocations are reserved for all public egress network usage. Devices with individual bandwidth metering and pool-based metering are all measured unless the device is ordered on the private network only.

Bandwidth allocation is a threshold where usage below the threshold is free or included, while usage in excess of the threshold is billed as a bandwidth overage. Bandwidth overages are billed individually per server or device, unless they participate in a bandwidth pool.

Devices added to a bandwidth pool contribute both their bandwidth allocation and bandwidth usage to form aggregated totals for the pool. If the pool usage exceeds the total pool allocation, the account owner is billed a consolidated pool overage fee.

## About device bandwidth
{: #bs-about-bw}

You can manage each device's bandwidth allocation. When you provision certain devices, you can select the amount of bandwidth that you want to allocate to that device. For each device, you pay for a fixed amount of bandwidth allocation during a billing cycle, and receive a notification when the device is at risk of overage for the billing cycle. For more information, see [Adding Bare Metal Server bandwidth](/docs/bandwidth-services?topic=bandwidth-services-adding-bare-metal-server-bandwidth) and [Adding virtual server instance bandwidth](/docs/bandwidth-services?topic=bandwidth-services-adding-virtual-server-insance-bandwidth).

When the bandwidth usage on a device reaches 85% of its total allocation, the account owner receives notifications.
{: note}

IBM charges for some firewall bandwidth services. For example, the Hardware Firewall (shared) product is not metered for bandwidth. The Fortigate Security Appliance 10G does receive an included bandwidth allocation, and is charged for egress bandwidth overages after that allocation has been exceeded. Additionally, these products can reduce total bandwidth usage by limiting the traffic that servers must respond to. Because monthly server bandwidth is recorded at the server switch port, traffic that is blocked by the hardware firewall is not counted against your monthly allocations, eliminating the need to pay for unwanted traffic. For more information, see [About Hardware Firewall](/docs/hardware-firewall-shared?topic=hardware-firewall-shared-about-hardware-firewall-shared-).

For Citrix Netscaler VPX appliances, you can purchase larger allocations of bandwidth at a reduced cost compared to the overage rate. For more information, see [Ordering a Citrix Netscaler VPX](/docs/citrix-netscaler-vpx?topic=citrix-netscaler-vpx-getting-started#ordering-a-citrix-netscaler-vpx).

## About bandwidth pools
{: #bs-about-bw-pools}

Bandwidth pooling optimizes your bandwidth usage by "pooling" all of the bandwidth of individual servers together into a bandwidth pool.

The bandwidth usage of devices in a bandwidth pool is summed up as a whole, and overages are calculated only if the total bandwidth of all servers exceeds the total allocated bandwidth for all servers. For example, if a bandwidth pool had five servers, each with 2000 GB of bandwidth, and one server used 3000 GB of bandwidth while the other used only 1500 GB of bandwidth in a billing cycle, you are not billed for a pool overage. Your total usage would be 9000 GB and your total allocated bandwidth would be 10000 GB. You would receive a notification after 8,500 GB of bandwidth usage.  
 
Notifications are sent to the account owner when the devices in the pool collectively use 85% of the pool's allotted bandwidth. 
{: note}

Bandwidth pools are beneficial when you have devices with variable month-to-month usage. In months during which the device uses little bandwidth, adding a device's individual bandwidth allocation to a bandwidth pool can prevent that device's bandwidth allocation from going to waste. In months during which the device risks exceeding its individual allocation, including the device in the bandwidth pool can prevent the device from receiving an overage fee. Bandwidth pools are defined geographically. 

Certain actions and devices are not permitted in bandwidth pooling:
- devices billed hourly (fully metered) are not eligible for bandwidth pooling
- devices with unlimited bandwidth plans are not eligible for bandwidth pooling
- pool-to-pool device moves are not permitted in the same billing period 

Devices billed hourly (fully metered) and devices with unlimited bandwidth are not eligible for bandwidth pooling. 
{: important}

For more information, see [Creating bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-create-ibm-cloud-bandwidth-pools).

## About scheduled devices
{: #bp-about-scheduled-devices}

When you delete a bandwidth pool or remove a device from a bandwidth pool, the deletion and removal aren't instantaneous. These actions are scheduled to take place on the date of your next billing anniversary. For more information, see [Deleting bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-delete-bw-pools) and [Removing devices from bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-remove-devices-from-bw-pools).

In the time between your requests and the completion of these requests on your billing anniversary, you can unschedule your requests. For more information, see [Unscheduling deletion of bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-unscedule-deletion-bw-pools) and [Unscheduling device removal from bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-unschedule-device-removal-from-bw-pools). 

## Use cases
{: #bw-services-use-cases}

The following use cases describe common situations for managing bandwidth services. 

### Use case 1: Responding to a device overage notification
{: #bw-how-to-respond-device-overage}

In this scenario, you receive a notification that your device used 85% of its allocated bandwidth. You have two options for how to respond to this notification. 

1. Do nothing and let your device continue to use bandwidth until the end of your billing cycle. If your device uses more than its allocated bandwidth, you are charged an overage fee for this device.
1. Upgrade the bandwidth on this individual server. The upgrade applies instantly, and the cost associated with this upgrade applies to your current monthly billing cycle. This prevents an overage fee on your server. 

### Use case 2: Responding to a pool overage notification
{: #bw-how-to-respond-pool-overage}

In this scenario, you receive a notification that the devices in your bandwidth pool used 85% of their collective allocated bandwidth. You have three options for how to respond to this notification. 

1. Do nothing and let the devices in your bandwidth pool continue to use bandwidth until the end of your billing cycle. If your devices use over their allocated bandwidth, you are charged an overage fee for your bandwidth pool.
1. Decide whether purchasing additional bandwidth for any one of the given devices in your bandwidth pool is the right approach. The upgrade applies instantly and the cost associated with this upgrade applies to your current monthly billing cycle. This individual bandwidth allocation is added to the collective bandwidth allocation for your bandwidth pool. For more information, see [Creating bandwidth pools](/docs/bandwidth-services?topic=bandwidth-services-how-to-create-ibm-cloud-bandwidth-pools).
1. Add more devices to your bandwidth pool to increase the total aggregated bandwidth limit of the pool by the individual allocated bandwidth amount of the new device. Adding a device to the pool instantly increases the total aggregated bandwidth limit of your pool. You can't remove the device from the pool until the end of the bandwidth pool's billing cycle.  
