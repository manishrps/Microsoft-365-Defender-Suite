## Lab 10 - Configure App Access Policies 

## Lab scenario

App Access Policies within the Microsoft 365 Defender suite involves setting rules and controls to manage how applications are accessed and used within an organization's digital environment. By specifying access controls, such as limiting app usage to certain devices, locations, or user groups, organizations can strengthen their security posture and protect sensitive data from unauthorized access or misuse.

## Lab objectives (Duration:  minutes)

In this lab, you will complete the following tasks:

- Task 1: Configure integration with Microsoft Entra ID
- Task 2: Create App Access Policies

## Architecture Diagram

### Task 1: Configure integration with Microsoft Entra ID

1. Navigate to Azure Portal, in **Search resources, services and docs** search and select for **Microsoft Entra ID**.

   ![Picture 1](../Media/image_41.png)

1. From the left-hand navigation pane, under **Manage**, select **Security**.

1. From the left-hand navigation pane, under **Protect**, select **Conditional Access**.

1. Select **+ Create new policy**.

1. Enter a policy name, **MyTest**.

1. Under **Users**, select **0 users and groups selected**, under **Include**, select **Select users and groups**.

   ![Picture 1](../Media/image_43.png)

1. select **Users and groups**.
Choose your user account for the lab tenant and select **Select**.

   ![Picture 1](../Media/image_45.png)
   ![Picture 1](../Media/image_44.png)

1. Under Target resources, select **No target resources selected**, under **Include**, select **Select apps**,under **Select** choose **None**, and then choose **Microsoft Forms**, and select **Select**.

   ![Picture 1](../Media/image_46.png)

1.  Under **Access controls**, under **Session**, select **0 controls selected**. Select the **Use Conditional Access App Control** box, select the drop-down and select **Monitor only (Preview)**, and select **Select**.

    ![Picture 1](../Media/image_47.png)

1. Under **Enable policy**, select **On**, and select **Create**.

## Task 3 - Log into Microsoft 365 and validate that conditional access is monitoring

1. Launch a new InPrivate browsing window, and browse to https://www.microsoft365.com/.

1. Select Sign in and log in them.

1.    


