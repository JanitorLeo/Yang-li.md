# **Standard Operating Procedure**
**[MITT]**  
**[130 Henlow Bay, Winnipeg, MB R2Y 1G4]**  
**[204 989 6500]**

**Version:** 1.0  
**Written by:** [Yang Li]  
**Approved by:** [Felix]  
**Date:** [11/22/2024]  

---

## **Purpose**
The purpose of this SOP is to provide IT personnel with a clear and structured process for setting up a Windows Server. This document ensures consistency, security, and efficiency in server deployment across the organization.

---

## **Application**
This SOP applies to all IT staff responsible for deploying new Windows Server instances. It is intended for use in scenarios such as new server installations, system upgrades, or disaster recovery implementations.

---

## **Definitions**
- **Windows Server**: A server operating system developed by Microsoft for enterprise-level management, storage, and application hosting.
- **ISO**: An image file format used for distributing operating systems.
- **Active Directory (AD)**: A directory service developed by Microsoft for Windows domain networks.
- **GUI**: Graphical User Interface, the visual interface of an operating system.
- **Core Installation**: A minimal installation option without a GUI, offering enhanced performance and security.

---

## **Procedure Steps**

### **Step 1: Prepare Installation Media**
1. Download the appropriate Windows Server ISO from the Microsoft website.
2. Create a bootable USB or DVD using tools like **Rufus** or mount the ISO for a virtual machine.

### **Step 2: Boot and Begin Installation**
1. Insert the installation media into the target machine.
2. Restart the machine and access the boot menu (commonly via **F2**, **F12**, or **Del**).
3. Select the installation media as the boot device.

### **Step 3: Install Windows Server**
1. Choose the language, time format, and keyboard layout, then click **Next**.
2. Select **Install Now** and enter the product key if prompted.
3. Choose the appropriate server edition and installation type (GUI or Core).
4. Configure the disk partition and proceed with installation.

### **Step 4: Perform Initial Setup**
1. After installation, log in using the Administrator account.
2. Configure a static IP address through **Network Settings**.
3. Rename the server for identification purposes (e.g., `Server01`).
4. Join the server to the domain if required.

### **Step 5: Update and Secure**
1. Use **Windows Update** to install the latest patches and security updates.
2. Configure Windows Firewall with necessary rules.
3. Install antivirus software or activate Microsoft Defender.
4. Disable unnecessary services via **Services.msc**.

### **Step 6: Add Server Roles**
1. Open **Server Manager** and select **Add roles and features**.
2. Choose the roles required for your environment (e.g., Active Directory, DNS, DHCP).
3. Complete the role-specific configuration.

### **Step 7: Validation and Testing**
1. Verify network connectivity using tools like `ping`.
2. Test server functionality by checking role-specific operations (e.g., domain controller services).
3. Inspect logs in **Event Viewer** for potential issues.

---

## **Resources**
- **Microsoft Documentation**: [docs.microsoft.com](https://docs.microsoft.com)
- **ISO Creation Tools**: [Rufus](https://rufus.ie)
- **Server Role Tutorials**: [Server Manager Tutorials](https://docs.microsoft.com/en-us/windows-server/get-started/)

---
