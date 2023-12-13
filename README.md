# EntraID Role Best Practices
This is for determining the best practices and assigning least-privilege for all Entra ID and Defender XDR roles.

# Overview

## Links and Resources

# Roles


## Defender XDR 


# Microsoft Defender XDR Role-Based Access Control

Title: **Security Role - Tier 1**

Tier: **One**

# Permissions
This role is configured under Microsoft Defender XDR's RBAC permissions. The role will have general analyst capabilities.

## Security Operations
### Security Data
* Select Custom Permissions
    * ✓ Security Data Basics (Read)
    * ✓ Alerts (Manage)
    * ✓ Response (Manage)
    * ✓ Basic Live Response (Manage)
    * ✓ File Collection (Manage)
    * ✓ Email Quarantine (Manage)

_Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information._

### Raw Data (Email and Collaboration)
* Select Custom Permissions
  * ✓ Email Message Headers (Read)
  * ✓ Email Content (Read)
 
_Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information._

## Security Posture
### Posture Management
* Select Custom Permissions
    * ✓ Vulnerability Management (Read)
    * ✓ Exception Handling (Manage)
    * ✓ Remediation Handling (Manage)
    * ✓ Application Handling (Manage)
    * ✓ Secure Score (Read)
    * ✓ Secure Score (Manage)

_Secure Score (Manage) can be restricted depending on your organization's needs._


## Authorization and Settings
### Authorization
* ✓ Read and Manage

_Some organizations may opt to restrict Authorization to read-only for Tier 1 analysts, as this could impact rule logic significantly if device groups are heavily utilized._

### Security Settings
* Select Custom Permissions
  * ✓ Detection Tuning (Manage)
  * ✓ Core Security Settings (Read)
 
_Some organizations may want to restrict detection tuning to a higher role as it can have significant impacts on false negatives._


### System Settings
* ✓ Read-only (Defender for Office, Defender for Identity)

_Granting the ability to see settings may give the analyst a better idea of the infrastructure and how things work. They cannot change anything. Your organization may have different needs._  




# Microsoft Defender XDR Role-Based Access Control

Title: **Security Role - Tier 2**

Tier: **Two**

# Permissions
This role is configured under Microsoft Defender XDR's RBAC permissions. The role will have more manage permissions than tier 1 does but is not able to change many settings.

## Security Operations
### Security Data
* Select Custom Permissions
    * ✓ Security Data Basics (Read)
    * ✓ Alerts (Manage)
    * ✓ Response (Manage)
    * ✓ Basic Live Response (Manage)
    * ✓ Advanced Live Response (Manage)
    * ✓ File Collection (Manage)
    * ✓ Email Quarantine (Manage)
    * ✓ Email Advanced Actions (Manage)

_Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information._

### Raw Data (Email and Collaboration)
* Select Custom Permissions
  * ✓ Email Message Headers (Read)
  * ✓ Email Content (Read)
 
_Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information._

## Security Posture
### Posture Management
* Select Custom Permissions
    * ✓ Vulnerability Management (Read)
    * ✓ Exception Handling (Manage)
    * ✓ Remediation Handling (Manage)
    * ✓ Application Handling (Manage)
    * ✓ Security Baselines Assessment (Manage)
    * ✓ Secure Score (Read)
    * ✓ Secure Score (Manage)

_Secure Score (Manage) can be restricted depending on your organization's needs._


## Authorization and Settings
### Authorization
* ✓ Read and Manage

_Some organizations may opt to restrict Authorization to read-only for Tier 1 analysts, as this could impact rule logic significantly if device groups are heavily utilized._

### Security Settings
* Select Custom Permissions
  * ✓ Detection Tuning (Manage)
  * ✓ Core Security Settings (Read)
  * ✓ Core Security Settings (Manage)
 
_Some organizations may want to restrict detection tuning to a higher role as it can have significant impacts on false negatives._


### System Settings
* ✓ Read-only (Defender for Office, Defender for Identity)

_Granting the ability to see settings may give the analyst a better idea of the infrastructure and how things work. They cannot change anything. Your organization may have different needs._  



# Microsoft Defender XDR Role-Based Access Control

Title: **Security Role - Tier 3**

Tier: **Three**

# Permissions
This role is configured under Microsoft Defender XDR's RBAC permissions. This role is used by senior/tier 3 analysts and engineers and has permission to do most everything in the Defender XDR platform.

**Note: Selecting "All read and manage permissions" at the top of the page will blank out all other permissions and assign them all. Below I have listed all of the permissions granted for tracking purposes.**

![image](https://github.com/CHAS-Health/EntraID-Role-Best-Practices/assets/8816079/bac071b3-d766-42cc-b12e-452161c24229)

## Security Operations
### Security Data
* All read and manage permissions
    * ✓ Security Data Basics (Read)
    * ✓ Alerts (Manage)
    * ✓ Response (Manage)
    * ✓ Basic Live Response (Manage)
    * ✓ Advanced Live Response (Manage)
    * ✓ File Collection (Manage)
    * ✓ Email Quarantine (Manage)
    * ✓ Email Advanced Actions (Manage)

### Raw Data (Email and Collaboration)
  * ✓ Email Message Headers (Read)
  * ✓ Email Content (Read)
 
_Email message permissions are entirely dependent on your organization's philosophy, structure, and job descriptions. Some organizations may not want your junior analysts to be able to read email information._

## Security Posture
### Posture Management
* All read and manage permissions
    * ✓ Vulnerability Management (Read)
    * ✓ Exception Handling (Manage)
    * ✓ Remediation Handling (Manage)
    * ✓ Application Handling (Manage)
    * ✓ Security Baselines Assessment (Manage)
    * ✓ Secure Score (Read)
    * ✓ Secure Score (Manage)

## Authorization and Settings
### Authorization
* ✓ Read and Manage

_Some organizations may opt to restrict Authorization to read-only for Tier 1 analysts, as this could impact rule logic significantly if device groups are heavily utilized._

### Security Settings
* All read and manage permissions
  * ✓ Detection Tuning (Manage)
  * ✓ Core Security Settings (Read)
  * ✓ Core Security Settings (Manage)
 

### System Settings
* ✓ Read and Manage



## Entra ID

## Cloud App Security
