---

copyright:
  years: 2022
lastupdated: "2022-11-30"

keywords: bandwidth services, bandwidth pools

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# FAQs for bandwidth services
{: #faqs}

You can review answers to some frequently asked questions about bandwidth services.
{: shortdesc}

## How are bandwidth services priced?
{: #price-points}
{: faq}

* Public bandwidth egress (or bandwidth allocation) pricing depends on regions as indicated in **Pricing plans by region** on the [Bandwidth packages from IBM Cloud](https://www.ibm.com/cloud/bandwidth){: external} website.
* Public bandwidth usage over GB allocation is charged per GB.  
 
## What IMS permissions do I need to view and change bandwidth allocations (or add and remove devices to/from bandwidth pools)?
{: #bw-permissions}
{: faq}
 
The `BANDWIDTH_MANAGE` IMS infrastructure classic permission is the only required permission for bandwidth services. This permission enables you to perform the following actions:
 - Create a bandwidth pool
 - Move a device into or out of a pool
 - Void a device’s move into a pool
 - Cancel a pool 

Certain actions pertaining to bandwidth pools, including visibility, may be constrained based on device-level permission. Reconcile your device-level permissions on specific devices to manage their bandwidth and membership in pools.
{: note}
 
## Is there an additional cost for bandwidth pools?
{: #bw-pool-cost}
{: faq}

Yes, there's a $25 USD per device fee to the pool per month. The pool itself doesn’t have an overhead cost of $25 per month. For example, a $150 server in the pool incurs a $25 one-time fee and $25 per month for as long as the device is in the pool. If you later decide to remove a device from a pool, the device continues to contribute to the pool cost until the end of the billing cycle.
 
## Why don't I see the same number of devices as displayed on the devices count?
{: #bw-device-count}
{: faq}

This issue might be due to permission restrictions because some users do not have permission to view specific devices. This issue could also be the result of devices that were reclaimed in the middle of the billing cycle, but are still contributing to the cost of the pool.
 
## What kind of devices generate bandwidth?
{: #bw-devices-generating-bandwidth}
{: faq}

Compute devices consume bandwidth. For example, devices that generate bandwidth include bare metal servers, virtual servers, firewalls (FSA 10G), and Netscaler devices.

## Why doesn't the allocation display the same value that I ordered?
{: #bw-allocation-value-differs}
{: faq}

The allocation shown is related to the proration policy. For example, let's say that you order 20 TB of bandwidth on the 15th of the month. The allocation shown on the bandwidth summary page will show 10 TB until the next billing cycle. Then, the allocation will display the full amount of what was ordered.

## What is the maximum number of devices that I can attach to a bandwidth pool?
{: #bw-max-number-vsi}
{: faq}

You can attach an unlimited number of devices to a bandwidth pool.
