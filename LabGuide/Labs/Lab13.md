## Lab 13 - Deploy Domain Controller 

## Lab scenario

A Domain Controller (DC) is a vital component in a Windows-based network that manages security, authentication, and access control. It runs the Active Directory Domain Services (AD DS) role, storing user account information, authenticating user logins, managing permissions, and organizing network resources like computers, printers, and files into a hierarchical structure. Essentially, it acts as a centralized hub, controlling and coordinating access to the network's resources, ensuring security, and enforcing policies across the domain.

## Lab objectives (Duration: minutes)

In this lab, you will complete the following tasks:
- Task 1.1: Configure VM with Static IP Addresses
- Task 1.2: Install Active Directory Domain Services

## Architecture Diagram

### Task 1: Deploy Domain Controller 

#### Task 1.1 : Configure VM with Static IP Addresses

Domain controllers need a static IP address and the DNS pointing to itself. For on-premises DCs you would just go into the NIC settings and manually configure the IP settings. With Azure VMs it’s recommended to set this at the Virtual Network Interface.

1. Go to **svm-<inject key="DeploymentID" enableCopy="false" /></inject>** virtual machine. In the left-hand menu for your VM under settings click on **Networking**.Now click on the Network Interface for the VM **svm-<inject key="DeploymentID" enableCopy="false" /></inject>-nic**.

   ![Picture 1](../Media/dc19.png)

2. Click on **IP Configurations** in the left menu under settings. Next click on **ipconfig1** under IP configurations.

3. Change the IP from **Dynamic** to **Static** and enter the IP address you want the domain controller to have, it must be an IP from the subnet you assigned to your virtual network like 10.0.0.4. Click **Save**.

   ![Picture 1](../Media/dc20.png)

4. Go back to the Network Interface and click on **DNS servers**. Set the DNS server to the IP address of the domain controller.

   ![Picture 1](../Media/dc21.png)

#### Task 1.2 : Install Active Directory Domain Services

With a VM pre-created and the IP settings configured we can move forward with installing Active Directory on the server.
1. From the jump VM. Search for **Server Manager** from the start menu and select it. Go to the server manager and click on **Add roles and features**.

   ![Picture 1](../Media/dc1.png)

2. You will be directed to **Before you begin** tab. Click **Next**.

   ![Picture 1](../Media/dc2.png)

3. In the **Installation type** tab, select **Role-based or feature-based installation** and click **Next**.

   ![Picture 1](../Media/dc3.png)

4. In the **Server Selection** tab, select **Select a server from the server pool** and then select the hostname of your server i.e. **svm-<inject key="DeploymentID" enableCopy="false" /></inject>** and click **Next**.

   ![Picture 1](../Media/dc4.png)

5. Under **Server Roles** tab, select **Active Directory Domain Services**. You will get a pop-up to add additional features. Click **Add Features** then Click **Next**.

   ![Picture 1](../Media/dc5.png)

   ![Picture 1](../Media/dc6.png)

6. Now, under **Features**, you will see additional features that we can add, as no features need to be added for now so click **Next**.

   ![Picture 1](../Media/dc7.png)

7. From the **Active Directory Domain Service** tab, Click **Next**.

   ![Picture 1](../Media/dc8.png)

8. In the **Confirm installation selections** tab, Click **Install**.

   ![Picture 1](../Media/dc9.png)

9. When finished click the flag icon in the upper right corner and click on **Promote this server to a domain controller**.

10. Now a new tab will open of Deployment configuration. Click on **Add a new forest**. Under **Root domain name** provide the domain which you can find in the Environment Details tab i.e. You can use the domain name which is present after the **@** <inject key="AzureAdUserEmail"></inject>.

   ![Picture 1](../Media/dc11.png)

11. Under **Domain Controller Options** tab, keep the default settings and provide a DSRM password and click **Next**.

   ![Picture 1](../Media/dc12.png)

12. In the **DNS Options** tab, Click **Next**.

13. In the **Additional Options** tab, **The NetBIOS domain name** will be automatically populated and click **Next**.

   ![Picture 1](../Media/dc13.png)

14. In **Paths** tab, keep the default paths as specified for Database folder, Log files folder and SYSVOL folder and click **Next**.

   ![Picture 1](../Media/dc14.png)

15. In **Review Options** tab, Review your settings and click **Next**.

   ![Picture 1](../Media/dc15.png)

16. In **Prerequisites Check** tab, You will see All prerequisite checks passed successfully. Click on **Install**

   ![Picture 1](../Media/dc16.png)

## Review
In this lab, you will complete the following tasks:
- Configure VM with Static IP Addresses
- Install Active Directory Domain Services

