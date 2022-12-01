---

copyright:
  years: 2022
lastupdated: "2022-10-30"

keywords: bandwidth services, bandwidth pools

subcollection: bandwidth-services

---

{{site.data.keyword.attribute-definition-list}}

# Managing permissions 
{: #bw-services-required-permissions}

The bandwidth manage IMS infrastructure classic permission is the only required permission for bandwidth services. Certain actions pertaining to bandwidth pools, including visibility, may be constrained based on device level permission. Reconcile your device level permissions on specific devices to manage their bandwidth and membership in pools.
{: shortdesc}

## IMS infrastructure classic required permission
{: #bw-services-required-ims-permission}

There is one infrastructure classic permission is required for bandwidth services. The **BANDWIDTH_MANAGE** permission is required for permitting a user to perform the following actions:
- Create a bandwidth pool
- Move a device into or out of a pool
- Void a device’s move into a pool
- Cancel a pool

The BANDWIDTH_MANAGE IMS infrastructure classic permission is the only required permission for bandwidth services. 
{: important}

## IAM permissions 
{: #bw-services-optional-iam-permissions}

To grant a user permission to perform different actions on a device, follow these steps:

1. Log in to the [Access (IAM)](/iam/users){: external} page in the {{site.data.keyword.cloud}} console.
1. Select the user's name and edit their permissions. 

A user's account permissions determine what actions they can perform on a device. 
{: important}
