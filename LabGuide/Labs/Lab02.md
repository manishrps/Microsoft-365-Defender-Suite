## Lab 02 - Configure Email Authentication

## Lab scenario

Email authentication (also known as email validation) is a group of standards that tries to stop email messages from forged senders (also known as spoofing). Microsoft 365 uses the following standards to verify inbound email:SPF, DKIM, DMARC.

## Lab objectives (Duration: minutes)


In this lab, you will complete the following tasks:
- Task 1: Configure DMARC For MOERA Domain.

## Architecture Diagram

### Task 1: Configure DMARC For MOERA Domain

1. Open the Microsoft 365 admin center at https://admin.microsoft.com.

1. On the left-hand navigation, select **Show All**.

1. Expand **Settings** and press **Domains**.

   ![Picture 1](../Media/image_14.png)

1. Select your tenant domain.

1. On the page that loads, select **DNS records**.

1. Select **+ Add record**.

   ![Picture 1](../Media/image_15.png)

1. A flyout will appear on the right. Ensure that the selected Type is **TXT** (Text).

1. Add as **TXT name**, **TXT value** and **TTL**. 

1. Click on **Save**.

   ![Picture 1](../Media/image_16.png)

1. Back on the **DNS records** tab, the entry is listed.

   ![Picture 1](../Media/image_17.png)

## Review
In this lab, you will complete the following tasks:
- Configure DMARC For MOERA Domain.

