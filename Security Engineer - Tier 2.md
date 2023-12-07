#### [Back to main page](https://github.com/CHAS-Health/EntraID-Role-Best-Practices/tree/main#entraid-role-best-practices)

# Security Engineer - Tier 2
### Title: Security Engineer 2
### Tier: Two
Purpose: This role is specifically intended to be used by the level two engineer. In most mid-sized organizations, this is what is classified as your mid to senior level position and will have permissions to do most things. That being said, it is not a global admin nor does it have tenant level permissions.

# Microsoft Entra ID Role Assignments

#Attack Simulation Administrator
Users in this role can create and manage all aspects of attack simulation creation, launch/scheduling of a simulation, and the review of simulation results. Members of this role have this access for all simulations in the tenant.

| Permission | Description |
| --- | --- |
| `microsoft.office365.protectionCenter/attackSimulator/payload/allProperties/allTasks` | Create and manage attack payloads in Attack Simulator | 
| `microsoft.office365.protectionCenter/attackSimulator/reports/allProperties/read` | Read reports of attack simulation, responses, and associated training |
| `microsoft.office365.protectionCenter/attackSimulator/simulation/allProperties/allTasks` | Create and manage attack simulation templates in Attack Simulator |

	
## Authentication Administrator - Privileged
This role allows users to reset authentication settings such as password, change MFA authentication type, clear saved authentication credentials, revoke sign-ins, and more. This role specifically prevents the admin from resetting admin authentication. 
| Permission | Description |
| --- | --- |
| `microsoft.directory/users/authenticationMethods/create` | Update authentication methods for users |
| `microsoft.directory/users/authenticationMethods/delete` | Delete authentication methods for users - Privileged |
| `microsoft.directory/users/authenticationMethods/standard/restrictedRead` | Read standard properties of authentication methods that do not include personally identifiable information for users` |
| `microsoft.directory/users/authenticationMethods/basic/update` | Update basic properties of authentication methods for users - Privileged |
| `microsoft.directory/deletedItems.users/restore` | Restore soft deleted users to original state - Privileged |
| `microsoft.directory/users/delete` | Delete users - Privileged |
| `microsoft.directory/users/disable` | Disable Users - Privileged |
| `microsoft.directory/users/enable` | Enable Users - Privileged |
| `microsoft.directory/users/invalidateAllRefreshTokens` | Force sign-out by invalidating user refresh tokens - Privileged |
| `microsoft.directory/users/restore` | Restore deleted users |
| `microsoft.directory/users/basic/update` | Update basic properties on users |
| `microsoft.directory/users/manager/update` | Update manager for users |
| `microsoft.directory/users/password/update` | Reset passwords for all users - Privileged |
| `microsoft.directory/users/userPrincipalName/update` | Update User Principal Name of users - Privileged |
| `microsoft.azure.serviceHealth/allEntities/allTasks` | Read and configure Azure Service Health |
| `microsoft.azure.supportTickets/allEntities/allTasks` | Create and manage Azure support tickets |
| `microsoft.office365.serviceHealth/allEntities/allTasks` | Read and configure Service Health in the Microsoft 365 admin center |
| `microsoft.office365.supportTickets/allEntities/allTasks` | Create and manage Microsoft 365 service requests |
| `microsoft.office365.webPortal/allEntities/standard/read` | Read basic properties on all resources in the Microsoft 365 admin center |

## Cloud Device Administrator
This is a privileged role. Users in this role can enable, disable, and delete devices in Microsoft Entra ID and read Windows 10 BitLocker keys (if present) in the Azure portal. The role does not grant permissions to manage any other properties on the device.

##Intune Administrator

This is a privileged role. Users with this role have global permissions within Microsoft Intune Online, when the service is present. Additionally, this role contains the ability to manage users and devices in order to associate policy, as well as create and manage groups. For more information, see Role-based administration control (RBAC) with Microsoft Intune.

This role can create and manage all security groups. However, Intune Administrator does not have admin rights over Office groups. That means the admin cannot update owners or memberships of all Office groups in the organization. However, he/she can manage the Office group that he creates which comes as a part of his/her end-user privileges. So, any Office group (not security group) that he/she creates should be counted against his/her quota of 250.


| Actions | Description |
| --- | --- |
| `microsoft.directory/bitlockerKeys/key/read` | Read bitlocker metadata and key on devices |
| `microsoft.directory/contacts/create` | Create contacts |
| `microsoft.directory/contacts/delete` | Delete contacts |
| `microsoft.directory/contacts/basic/update` | Update basic properties on contacts |
| `microsoft.directory/deletedItems.devices/delete` | Permanently delete devices, which can no longer be restored |
| `microsoft.directory/deletedItems.devices/restore` | Restore soft deleted devices to original state |
| `microsoft.directory/devices/create` | Create devices (enroll in Microsoft Entra ID) |
| `microsoft.directory/devices/delete` | Delete devices from Microsoft Entra ID |
| `microsoft.directory/devices/disable` | Disable devices in Microsoft Entra ID |
| `microsoft.directory/devices/enable` | Enable devices in Microsoft Entra ID |
| `microsoft.directory/devices/basic/update` | Update basic properties on devices |
| `microsoft.directory/devices/extensionAttributeSet1/update` | Update the extensionAttribute1 to extensionAttribute5 properties on devices |
| `microsoft.directory/devices/extensionAttributeSet2/update` | Update the extensionAttribute6 to extensionAttribute10 properties on devices |
| `microsoft.directory/devices/extensionAttributeSet3/update` | Update the extensionAttribute11 to extensionAttribute15 properties on devices |
| `microsoft.directory/devices/registeredOwners/update` | Update registered owners of devices |
| `microsoft.directory/devices/registeredUsers/update` | Update registered users of devices |
| `microsoft.directory/deviceLocalCredentials/password/read` | Read all properties of the backed up local administrator account credentials for Microsoft Entra joined devices, including the password |
| `microsoft.directory/deviceManagementPolicies/standard/read` | Read standard properties on device management application policies |
| `microsoft.directory/deviceRegistrationPolicy/standard/read` | Read standard properties on device registration policies |
| `microsoft.directory/groups/hiddenMembers/read` | Read hidden members of Security groups and Microsoft 365 groups, including role-assignable groups |
| `microsoft.directory/groups.security/create` | Create Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/delete` | Delete Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/basic/update` | Update basic properties on Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/classification/update` | Update the classification property on Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/dynamicMembershipRule/update` | Update the dynamic membership rule on Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/members/update` | Update members of Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/owners/update` | Update owners of Security groups, excluding role-assignable groups |
| `microsoft.directory/groups.security/visibility/update` | Update the visibility property on Security groups, excluding role-assignable groups |
| `microsoft.directory/users/basic/update` | Update basic properties on users |
| `microsoft.directory/users/manager/update` | Update manager for users |
| `microsoft.directory/users/photo/update` | Update photo of users |
| `microsoft.azure.supportTickets/allEntities/allTasks` | Create and manage Azure support tickets |
| `microsoft.cloudPC/allEntities/allProperties/allTasks` | Manage all aspects of Windows 365 |
| `microsoft.intune/allEntities/allTasks` | Manage all aspects of Microsoft Intune |
| `microsoft.office365.organizationalMessages/allEntities/allProperties/read` | Read all aspects of Microsoft 365 Organizational Messages |
| `microsoft.office365.supportTickets/allEntities/allTasks` | Create and manage Microsoft 365 service requests |
| `microsoft.office365.webPortal/allEntities/standard/read` | Read basic properties on all resources in the Microsoft 365 admin center |

## Message Center Privacy Reader
Users in this role can monitor all notifications in the Message Center, including data privacy messages. Message Center Privacy Readers get email notifications including those related to data privacy and they can unsubscribe using Message Center Preferences. Only the Global Administrator and the Message Center Privacy Reader can read data privacy messages. Additionally, this role contains the ability to view groups, domains, and subscriptions. This role has no permission to view, create, or manage service requests.

| Permission | Description |
| --- | --- |
| `microsoft.office365.messageCenter/messages/read` | Read messages in Message Center in the Microsoft 365 admin center, excluding security messages
| `microsoft.office365.messageCenter/securityMessages/read` | Read security messages in Message Center in the Microsoft 365 admin center
| `microsoft.office365.webPortal/allEntities/standard/read` | Read basic properties on all resources in the Microsoft 365 admin center 

## Security Reader - Privileged
This is a privileged role. Users with this role have global read-only access on security-related feature, including all information in Microsoft 365 Defender portal, Microsoft Entra ID Protection, Privileged Identity Management, as well as the ability to read Microsoft Entra sign-in reports and audit logs, and in Microsoft Purview compliance portal. For more information about Office 365 permissions, see Roles and role groups in Microsoft Defender for Office 365 and Microsoft Purview compliance.

| Permission | Description |
| --- | --- |
| `microsoft.directory/accessReviews/definitions/allProperties/read` | Read all properties of access reviews of all reviewable resources in Microsoft Entra ID |
| `microsoft.directory/auditLogs/allProperties/read` | Read all properties on audit logs, excluding custom security attributes audit logs |
| `microsoft.directory/authorizationPolicy/standard/read` | Read standard properties of authorization policy |
| `microsoft.directory/bitlockerKeys/key/read` | Read bitlocker metadata and key on devices - Privileged |
| `microsoft.directory/deviceLocalCredentials/standard/read` | Read all properties of the backed up local administrator account credentials for Microsoft Entra joined devices, except the password |
| `microsoft.directory/domains/federationConfiguration/standard/read` | Read standard properties of federation configuration for domains |
| `microsoft.directory/entitlementManagement/allProperties/read` | Read all properties in Microsoft Entra entitlement management |
| `microsoft.directory/identityProtection/allProperties/read` | Read all resources in Microsoft Entra ID Protection |
| `microsoft.directory/namedLocations/standard/read` | Read basic properties of custom rules that define network locations |
| `microsoft.directory/policies/standard/read` | Read basic properties on policies |
| `microsoft.directory/policies/owners/read` | Read owners of policies |
| `microsoft.directory/policies/policyAppliedTo/read` | Read policies.policyAppliedTo property |
| `microsoft.directory/conditionalAccessPolicies/standard/read` | Read Conditional Access for policies |
| `microsoft.directory/conditionalAccessPolicies/owners/read` | Read the owners of Conditional Access policies |
| `microsoft.directory/conditionalAccessPolicies/policyAppliedTo/read` | Read the "applied to" property for Conditional Access policies |
| `microsoft.directory/crossTenantAccessPolicy/partners/templates/multiTenantOrganizationIdentitySynchronization/standard/read` | Read basic properties of cross tenant sync policy templates for multi-tenant organization |
| `microsoft.directory/crossTenantAccessPolicy/partners/templates/multiTenantOrganizationPartnerConfiguration/standard/read` | Read basic properties of cross tenant access policy templates for multi-tenant organization |
| `microsoft.directory/multiTenantOrganization/joinRequest/standard/read` | Read properties of a multi-tenant organization join request |
| `microsoft.directory/multiTenantOrganization/standard/read` | Read basic properties of a multi-tenant organization |
| `microsoft.directory/multiTenantOrganization/tenants/organizationDetails/read` | Read organization details of a tenant participating in a multi-tenant organization |
| `microsoft.directory/multiTenantOrganization/tenants/standard/read` | Read basic properties of a tenant participating in a multi-tenant organization |
| `microsoft.directory/privilegedIdentityManagement/allProperties/read` | Read all resources in Privileged Identity Management |
| `microsoft.directory/provisioningLogs/allProperties/read` | Read all properties of provisioning logs |
| `microsoft.directory/signInReports/allProperties/read` | Read all properties on sign-in reports, including privileged properties |
| `microsoft.azure.serviceHealth/allEntities/allTasks` | Read and configure Azure Service Health |
| `microsoft.networkAccess/allEntities/allProperties/read` | Read all aspects of Microsoft Entra Network Access |
| `microsoft.office365.protectionCenter/allEntities/standard/read` | Read standard properties of all resources in the Security and Compliance centers |
| `microsoft.office365.protectionCenter/attackSimulator/payload/allProperties/read` | Read all properties of attack payloads in Attack Simulator |
| `microsoft.office365.protectionCenter/attackSimulator/reports/allProperties/read` | Read reports of attack simulation, responses, and associated training |
| `microsoft.office365.protectionCenter/attackSimulator/simulation/allProperties/read` | Read all properties of attack simulation templates in Attack Simulator |
| `microsoft.office365.serviceHealth/allEntities/allTasks` | Read and configure Service Health in the Microsoft 365 admin center |
| `microsoft.office365.webPortal/allEntities/standard/read` | Read basic properties on all resources in the Microsoft 365 admin center |


## Service Support Administrator
Users with this role can create and manage support requests with Microsoft for Azure and Microsoft 365 services, and view the service dashboard and message center in the Azure portal and Microsoft 365 admin center.
| Permission | Description |
| --- | --- |
| microsoft.azure.serviceHealth/allEntities/allTasks | Read and configure Azure Service Health |
| microsoft.azure.supportTickets/allEntities/allTasks | Create and manage Azure support tickets |
| microsoft.office365.network/performance/allProperties/read | Read all network performance properties in the Microsoft 365 admin center |
| microsoft.office365.serviceHealth/allEntities/allTasks | Read and configure Service Health in the Microsoft 365 admin center |
| microsoft.office365.supportTickets/allEntities/allTasks | Create and manage Microsoft 365 service requests |
| microsoft.office365.webPortal/allEntities/standard/read | Read basic properties on all resources in the Microsoft 365 admin center |


			
