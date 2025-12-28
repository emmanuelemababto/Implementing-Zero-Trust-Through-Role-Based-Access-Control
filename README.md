# Azure Identity and Access Management 

# RBAC, Least Privilege, and Zero Trust

# Overview

This lab demonstrates how to manage administrator access in Azure using Microsoft Entra ID and Azure Role-Based Access Control (RBAC). The focus is on preventing over-privileged access by separating cloud resource permissions from identity-level administrative roles using least-privilege and Zero Trust principles.


# Objectives

Create admin and standard users in Microsoft Entra ID

Manage access using security groups

Apply RBAC at the subscription level

Prevent identity privilege escalation

Validate access through testing


# Tools Used

Microsoft Entra ID

Azure RBAC (IAM)

Azure Subscription

Azure Portal

Audit and sign-in logs


# Implementation

Created admin and standard users in Microsoft Entra ID

Created a security group (Cloud-Sec-Admins)

Added admin users to the group

Assigned the Reader role to the group at the subscription level

Tested permissions to confirm access boundaries


# Validation

Admins can:

View and manage Azure resources

View audit logs

Grant scoped access

Admins cannot:

Create Global Administrator accounts

Elevate identity privileges

Admins can create standard users within scoped groups.


# Outcome

Secure cloud resource access without over-permissioning

Clear separation between cloud management and identity administration

Reduced identity security risk

Enterprise-aligned IAM design


# Lessons Learned

RBAC should be assigned to groups, not individual users

Global Administrator roles should not be assigned to groups

Identity privileges must be separated from cloud resource access

Least privilege and Zero Trust reduce attack surface

Permission testing is critical

# ScreenShots
<img width="960" height="540" alt="creating new azure user" src="https://github.com/user-attachments/assets/da401c27-4c19-495a-8fa5-0fac149df2e0" />

<img width="960" height="504" alt="adding a read role for IT-admin establish zero trust achitecture" src="https://github.com/user-attachments/assets/0deab654-0656-4f39-ab2b-a9ac83096d02" />

<img width="960" height="504" alt="verifying if admin group was created  and if IT- admin user exist in the group" src="https://github.com/user-attachments/assets/da2d2dc9-c6a4-48f1-8d51-1b2e32aa3f96" />

<img width="960" height="504" alt="adding It admin to IT-group" src="https://github.com/user-attachments/assets/884a2931-482e-403d-9302-c0a22cd650b0" />

<img width="1012" height="504" alt="creating an admin group" src="https://github.com/user-attachments/assets/49854139-94c0-4c55-87cf-6f5dca26baba" />

<img width="960" height="504" alt="verifying user exist" src="https://github.com/user-attachments/assets/980e73de-fe63-4c99-ae32-4f0a2a282b37" />

<img width="990" height="504" alt="admin user can create users after giving him a user administrative role " src="https://github.com/user-attachments/assets/a1cba44b-8817-42b7-a76d-3d2dffcdc734" />

<img width="960" height="504" alt="it-admin user cannot create any internal user" src="https://github.com/user-attachments/assets/f6f9ed7b-fbf0-47db-9fce-e1e0336eb6ad" />

<img width="997" height="520" alt="IT-admin user signed in" src="https://github.com/user-attachments/assets/580dd790-cc2b-4b4d-8893-08f07ad939ee" />

<img width="976" height="504" alt="verifying user It-admin  privelege role only applies  to  the admin in the group" src="https://github.com/user-attachments/assets/4e59aa8d-d2fb-4488-a8a2-e994b8332e30" />

<img width="960" height="504" alt="applying the role just to IT-Admin user" src="https://github.com/user-attachments/assets/eca44d02-0d5f-4387-9374-a6af337b8bc0" />

<img width="960" height="504" alt="Assigning a privilege role to admin user in the IT group" src="https://github.com/user-attachments/assets/0ff5705f-6b75-4c57-b75c-effb06d7f902" />




I built an Azure IAM lab using Entra ID and RBAC to enforce least privilege. Admin access was managed through groups, allowing cloud resource management while preventing identity privilege escalation. This reflects real enterprise identity governance practices.
