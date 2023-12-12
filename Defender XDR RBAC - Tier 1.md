# Microsoft Defender XDR Role-Based Access Control
### Title: Security Role - Tier 1
### Tier: One

# Permissions
This role is configured under Microsoft Defender XDR's RBAC permissions. The role will have general analyst capabilities.

## Security Operations
### Security Data
* Select Custom Permissions
    * Security Data Basics (Read)
    * Alerts (Manage)
    * Response (Manage)
    * Basic Live Response (Manage)
    * File Collection (Manage)
    * Email Quarantine (Manage)
    * 
`note:` Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information.
  
### Raw Data (Email and Collaboration)
* Select Custom Permissions
  * Email Message Headers (Read)
  * Email Content (Read)

`note:` Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information.

## Security Posture
### Posture Management
* Select Custom Permissions
    * Vulnerability Management (read)
    * Exception Handling (manage)
    * Remediation Handling (manage)
    * Application Handling (manage)
    * Secure Score (read)
    * Secure Score (manage)
    * 
 `note:` Secure Score (manage) can be restricted depending on your organization's needs.


## Authorization and Settings
### Authorization
* Read and Manage

### Security Settings
* Select Custom Permissions
  * Detection Tuning (manage)
  * Core Security Settings (read)
 
`note:` Some organizations may want to restrict detection tuning to a higher role as it can have significant impacts on false negatives.

### System Settings
* Read-only (Defender for Office, Defender for Identity)

`note:` Granting the ability to see settings may give the analyst a better idea of the infrastructure and how things work. They cannot change anything. Your organization may have different needs.
  



