## Lab 13 - Deploy Domain Controller 

## Lab scenario
In this lab you will explore about the *Deploying Domain Controller*.

## Lab objectives (Duration: minutes)

In this lab, you will complete the following tasks:
- Task 1.1: Configure VM with Static IP Addresses
- Task 1.1: Install Active Directory Domain Services

## Architecture Diagram

### Task 1: Deploy Domain Controller 

### Task 1.1 : Configure VM with Static IP Addresses

Domain controllers need a static IP address and the DNS pointing to itself. For on-premises DCs you would just go into the NIC settings and manually configure the IP settings. With Azure VMs it’s recommended to set this at the Virtual Network Interface.

1. Go to **svm-<inject key="DeploymentID" enableCopy="false" /></inject>** virtual machine. In the left-hand menu for your VM under settings click on **Networking**.Now click on the Network Interface for the VM **svm-<inject key="DeploymentID" enableCopy="false" /></inject>-nic**.
2. Click on **IP Configurations** in the left menu under settings. Next click on **ipconfig1** under IP configurations.
3. Change the IP from **Dynamic** to **Static** and enter the IP address you want the domain controller to have, it must be an IP from the subnet you assigned to your virtual network like 10.0.0.4. Click **Save**.
4. Go back to the Network Interface and click on **DNS servers**. Set the DNS server to the IP address of the domain controller.

### Task 1.2 : Install Active Directory Domain Services

1. With a VM pre-created and the IP settings configured we can move forward with installing Active Directory on the server.
2. From the jump VM. Search for **Server Manager** from the start menu and select it. Go to the server manager and click on **Add roles and features**.
3. You will be directed to **Before you begin** tab. Click **Next**.
4. In the **Installation type** tab, select **Role-based or feature-based installation** and click **Next**.
5. In the **Server Selection** tab, select **Select a server from the server pool** and then select the hostname of your server i.e. **svm-<inject key="DeploymentID" enableCopy="false" /></inject>** and click **Next**.
6. Under **Server Roles** tab, select **Active Directory Domain Services**. You will get a pop-up to add additional features. Click **Add Features** then Click **Next**.
7. Now, under **Features**, you will see additional features that we can add, as no features need to be added for now so click **Next**.
8. From the **Active Directory Domain Service** tab, Click **Next**.
9. In the **Confirm installation selections** tab, Click **Install**.
10. When finished click the flag icon in the upper right corner and click on **Promote this server to a domain controller**.
11. Now a new tab will open of Deployment configuration. Click on **Add a new forest**. Under **Root domain name** provide the domain which you can find in the Environment Details tab i.e. You can use the domain name which is present after the **@** <inject key="AzureAdUserEmail"></inject>.
12. Under **Domain Controller Options** tab, keep the default settings and provide a DSRM password and click **Next**.
13. In the **DNS Options** tab, Click **Next**.
14. In the **Additional Options** tab, **The NetBIOS domain name** will be automatically populated and click **Next**.
15. In **Paths** tab, keep the default paths as specified for Database folder, Log files folder and SYSVOL folder and click **Next**.
16. In **Review Options** tab, Review your settings and click **Next**.
17. In **Prerequisites Check** tab, You will see All prerequisite checks passed successfully. Click on **Install**



