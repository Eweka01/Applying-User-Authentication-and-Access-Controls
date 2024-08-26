# Applying User Authentication and Access Controls

**Author**: Osamudiamen Eweka  
**Course**: CYB-605-Z2 Principles of Cybersecurity  
**Institution**: Utica University

## Overview

This lab explores user authentication and access controls within a Windows Active Directory environment. Participants engage in hands-on exercises to create users, security groups, and configure access permissions using Microsoft Active Directory Domain Services. The lab emphasizes the critical role of access control mechanisms in protecting corporate assets, particularly in cloud environments where security threats are prevalent.

## Objectives

- Understand the use of Microsoft Active Directory Domain Services to manage authentication and access control.
- Learn to create and manage user accounts and security groups in a Windows environment.
- Configure access control lists (ACLs) to secure files and folders from unauthorized access.
- Compare and contrast Windows Security permissions with Windows Share permissions.
- Secure a TrueNAS file server using Active Directory and Samba for remote file sharing.

## Lab Setup

### Lab Environment Details

The lab setup includes the following key tools:

- **Active Directory Users and Computers (ADUC)**: A critical tool for managing user accounts and security groups in Active Directory.
- **PowerShell**: Used for automating administrative tasks, particularly in system management.
- **TrueNAS**: Provides Network-Attached Storage (NAS) solutions for file sharing and storage, integrated with Active Directory for authentication.

## Hands-On Demonstrations

### 1. Creating Users and Security Groups
Participants begin by creating user accounts and security groups using ADUC. Key groups include Developers, Managers, and HR, each corresponding to specific job roles within the organization. This step emphasizes the importance of managing access based on user roles to enhance security.

### 2. Configuring Security Permissions
Participants then create folders for each group (e.g., HRfiles, MGRfiles, DEVfiles) and configure security permissions using NTFS. Specific permissions are applied to ensure that only authorized users can access their designated folders, while inheritance from parent directories is disabled to maintain security granularity.

### 3. Verifying Authentication and Access Controls
In this phase, participants test the newly established permissions by logging in with various user accounts and attempting to access different folders. This process verifies the effectiveness of the configured access controls and ensures that permissions align with the principle of least privilege (PoLP).

## Applied Learning

### 1. Creating an SMB Share on TrueNAS
Participants configure a TrueNAS file server to serve as network-attached storage. The lab guides participants through creating datasets and applying Access Control Lists (ACLs) to manage access based on security groups created earlier in Active Directory. This integration of Samba with Active Directory demonstrates the importance of secure remote file sharing.

### 2. Verifying Access Controls on TrueNAS
After configuring the TrueNAS server, participants verify that access controls are functioning correctly by logging in as different users and attempting to access shared folders. Screenshots are captured to document successful and failed access attempts, providing visual confirmation of the applied security settings.

## Challenge and Analysis

Participants are tasked with integrating GG Studios’ workforce into the Active Directory environment following a corporate merger. This involves creating new security groups, user accounts, and configuring permissions on the TrueNAS file server. The process concludes with verifying that the new users have appropriate access to shared resources based on their roles.

## Conclusion

This lab emphasizes the importance of user authentication and access controls in securing organizational networks. Through hands-on experience with Active Directory and TrueNAS, participants gain practical skills in configuring and managing security permissions, ensuring that corporate resources are protected from unauthorized access. The lab highlights the critical role of access control in maintaining a robust cybersecurity posture.

## References

- Bruce, N., Lee, H. J., & Lee, S. (2014). Security analysis and improvements of authentication and access control in the internet of things. *Sensors*, 14(8), 14786–14805. https://doi.org/10.3390/s140814786
- Kim, D., & Solomon, M. G. (2021). *Fundamentals of Information Systems Security*. Jones & Bartlett Learning.
- Sdwheeler. (2023, June 28). What is PowerShell? - PowerShell. Microsoft Learn. https://learn.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7.4
- TrueNAS. (2023). TrueNAS core - world’s most popular open storage OS. https://www.truenas.com/truenas-core/

For a complete list of references, please refer to the full lab report.


## Documentation

For more details, you can refer to the full lab report: 
[User_Authentication_and_Access_Controls](https://github.com/user-attachments/files/16739361/lab.4.Applying_User_Authentication_and_Access_Controls_4e_-_Osamudiamen_Eweka.docx)

