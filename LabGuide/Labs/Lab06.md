## Lab 06 - Launch Phishing Simulation Campaigns. 

## Lab scenario

Phishing Simulation Campaigns in Microsoft 365 Defender involve creating fake phishing emails to test and educate users. These campaigns mimic real attacks, evaluating users' responses to improve their awareness. They're set up by crafting realistic emails, sent to targeted groups, and monitored for user interactions. Reports are generated to analyze user behavior and provide immediate feedback for learning. Continuous analysis helps adapt training to enhance security awareness, strengthening defences against actual phishing threats.

## Lab objectives (Duration: minutes)


In this lab, you will complete the following tasks:
- Exercise 1: Simulate a Phishing Attack.

## Architecture Diagram

### Exercise 1: Simulate a Phishing Attack.

1. Go to Microsoft Defender portal at https://security.microsoft.com.

1. Go to **Email & collaboration** > **Attack simulation training** > **Simulations** tab and Click on **Launch a Simulation**.

      ![Picture 1](../Media/image_18.png)
   
1. On the **Select technique** page, select **Credential Harvest** and Click on **Next**.

      ![Picture 1](../Media/image_19.png)
   
1. On the Name simulation page, configure the following settings:

   - **Name**: Enter a unique, descriptive name (**Credentials_Simulation**) for the simulation.
   - **Description**: Enter an optional detailed description for the simulation.
  When you're finished on the Name simulation page, select **Next**.

   ![Picture 1](../Media/image_20.png)

1. On the **Select payload and login page** page, you need to select **Reset Password** and Click on **Next**.

      ![Picture 1](../Media/image_22.png)

1.  On the **Target users** screen, Select **Include only specific users and groups** and Click **Add users**.

      ![Picture 1](../Media/image_23.png)

1.  Select for your user, click on **Add 1 User(s)**.

      ![Picture 1](../Media/image_24.png)

1. Click on **Next**.

      ![Picture 1](../Media/image_25.png)

1. On the **Exclude Users** page and click on **Next**.

      ![Picture 1](../Media/image_26.png)

1.  On the **Assign training** page Select the Recommended **Microsoft training experience** and **Assign training for me**, Select **Due Date** as **7 days after Simulation ends**, click on **Next**.

      ![Picture 1](../Media/image_27.png)

1. On the **Select Phish landing page**, select **Use landing pages from library** and **Payload Indicator**, Under *Global landing pages* select **Microsoft Landing Page Template 2** and click on **Next**.

      ![Picture 1](../Media/image_28.png)

1.  **Select end user notification** page, Select **Microsoft default notification (recommended)** and under the *Notifications* section, In  the  *Microsoft default notification Positive reinforcement notifications* select the **Deliver during simulations** and in *Microsoft default training reminder notification* select the **Twice a week**, Click on **Next**.

      ![Picture 1](../Media/image_29.png)

1. On the **Launch details** page, Click on **Next**.

      ![Picture 1](../Media/image_31.png)

1. In *Review Simulation* page, **Send a test** and click on **Submit**.

      ![Picture 1](../Media/image_32.png)

1. Click on **Done**.

      ![Picture 1](../Media/image_33.png)

1. It will navigate back to the **Attack Simulation training** page, where it shows the created **simulation**.

      ![Picture 1](../Media/image_34.png)

1. Click on the **Credentials_simulation** and navigate to the **Report** section.

      ![Picture 1](../Media/image_39.png)

1. Users will receive an email notification after some time. The Defender captures and records the user details when the user clicks on the URL, and respective training will be assigned to them.

      ![Picture 1](../Media/image_38.png)

1. Navigate back to the **Report** to check user activity.

      ![Picture 1](../Media/image_40.png) 

## Review
In this lab, you will complete the following tasks:
- Simulate a Phishing Attack.
   
