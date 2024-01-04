## Lab 14 - Setup Defender for Identity Sensors 

## Lab scenario

Defender for Identity Sensors within the Microsoft 365 Defender suite involves installing and configuring sensors on your on-premises domain controllers. These sensors play a crucial role in Defender for Identity (formerly Azure ATP), monitoring network traffic to detect and prevent threats related to identity and authentication within an organization's network.

## Lab objectives (Duration: minutes)

In this lab, you will complete the following tasks:
- Exercise 1: Tag apps as sanctioned or unsanctioned
- Exercise 2: Use the investigation tools

## Architecture Diagram

### Exercise 1: Tag apps as sanctioned or unsanctioned

1. To create a Defender for Identity workspace, Go to Microsoft Defender Portal, and from the left menu, select **Settings > Identities**.

   ![Picture 1](../Media/setupsensor1.png)

2. On the General tab, select **Directory services accounts**. To connect your on-premises environment, select **Add credentials**.

   ![Picture 1](../Media/setupsensor2.png)

3. In the Add credentials panel, enter Account name, Domain, and Password.

   ![Picture 1](../Media/setupsensor3.png)
