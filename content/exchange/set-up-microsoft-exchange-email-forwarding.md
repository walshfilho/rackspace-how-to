---
permalink: set-up-microsoft-exchange-email-forwarding/
audit_date: '2017-06-28'
title: Set up Microsoft Exchange email forwarding
type: article
created_date: '2017-06-07'
created_by: William Loy
last_modified_date: '2017-06-28'
last_modified_by: Nate Archer
product: Microsoft Exchange
product_url: exchange
---

You can configure a Microsoft Exchange mailbox to forward to another email address.

If you need to configure forwarding for a Rackspace Email mailbox, see [Set up forwarding for a Rackspace Email mailbox](/how-to/set-up-rackspace-email-forwarding/).

### Prerequisites

- **Applies to:** Administrator

- **Difficulty:** Moderate

- **Time needed:** Approximately 10 minutes to set forward / Additional 15 minutes for forward to enable

- **Tools required:** [Cloud Office Control Panel](https://cp.rackspace.com) access

For more information about prerequisite terminology, see [Cloud Office support terminology](/how-to/cloud-office-support-terminology).

- [Forward to a mailbox on the same domain](#forward-a-microsoft-exchange-mailbox-to-a-mailbox-on-the-same-domain)
- [Forward to an external domain's email address](#forward-a-microsoft-exchange-mailbox-to-an-external-domain's-email-address)
- [Forward to multiple email addresses](#forward-a-microsoft-exchange-mailbox-to-multiple-email-addresses)


### Forward to a mailbox on the same domain

Use these steps to forward email from your Microsoft Exchange address to another address on the same domain.

1. Log in to the [Cloud Office Control Panel](https://cp.rackspace.com/) using your Rackspace Cloud Office admin ID and password.
2. In the **Microsoft Exchange** section, click **Mailboxes**.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-1.png %}" />

3. Select the domain that contains the mailbox you would like to forward.
4. Click the mailbox you would like to forward from.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-2.png %}" />

5. Select the **Mail Forwarding** tab. On Mail Forwarding screen, select **Forward to an Exchange address within this domain**.
6. Select the address you want to forward email to from the list.
7. Select the **Save copies of forwarded email** option.

       <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-3.png %}" />

    If **Save a copy of forwarded email** is not checked, this mailbox will _not_ store any messages sent to it.

8. Click **Save**. Allow at least 15 minutes for the forward to enable.

### Forward a Microsoft Exchange mailbox to an external domain's email address

To forward to a mailbox with an external domain, use these steps to create an external contact for the external domain then forward your Exchange mailbox to that contact.

1. Log in to the [Cloud Office Control Panel](https://cp.rackspace.com/) using your Rackspace Cloud Office admin ID and password.
2. In the **Microsoft Exchange** section, select **Contacts**.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-contact-1.png %}" />

3. If you have multiple domains, select the domain that contains the mailbox you would like to forward.
4. Select **Add Contact**.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-contact-2.png %}" />

   Fill out the requested information in the fields provided.

    - **First Name and Last Name (optional):** Enter the first and last name of the new contact.
    - **Display Name:** Enter the name that is displayed in the Global Address List.
    - **Username:** Enter the **Contact address**. This is not a physical mailbox.
    - **External Email:** Enter the actual email address that you want to forward email to.

       <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-contact-3.png %}" />

6. Click **Save** to create the contact.
7. Click the **Mailboxes** tab.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-contact-4.png %}" />

8. In the mailbox list, click the mailbox name that you would like to forward.
9. Click the **Mail Forwarding** tab. On the Mail Forwarding screen, select **Forward to an Exchange address within this domain**.

   **Note:** Forwarding to an Exchange address within another domain on this account will work only if both domains are on the same Exchange server. If you are not sure if both domains are on the same Exchange server, the method of creating a contact will work regardless.

11. Select the **Save copies of forwarded email** option.

       <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-contact-6.png %}" />

    If **Save a copy of forwarded email** is not checked, this mailbox _not_ store any messages sent to it.

11. Click **Save**. Allow at least 15 minutes for the forward to enable.

### Forward a Microsoft Exchange mailbox to multiple email addresses

Use these steps to create a Microsoft Exchange **Distribution List** in order to forward to multiple email addresses.

Any address in your Distribution List that are not on the your domain need to be made into a contact before the external address can be added to the Distribution List. For instructions, see [Forward a Microsoft Exchange mailbox to an external domain's email address](#forward-a-microsoft-exchange-mailbox-to-an-external-domain's email-address).

1. Log in to the [Cloud Office Control Panel](https://cp.rackspace.com/) using your Rackspace Cloud Office admin ID and password.
2. In the **Microsoft Exchange** section, select **Lists**.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-1.png %}" />

3. Select the domain that contains the mailbox you would like to forward.

4. Select **Add Distribution List**.  

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-2.png %}" />

5. Fill out the required fields under **General**.

    - **Display Name:** Enter the name that is displayed in the Global Address List.
    - **Email Address:** Enter the **Distribution List Address**. This is not a physical mailbox. This is used forward to the multiple email addresses inside the selected **Distribution List**.
    - **Members:** Enter the members that you want receive a copy of email sent to the Distribution List.

    <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-3.png %}" />

6. In the **Advanced** section, select **Selected addresses on this domain** and select the address you plan to forward.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-4.png %}" />

7. Click **Create Distribution List**.  You will see the created list on the next screen. From this screen select the **Mailboxes** tab.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-5.png %}" />

8. In the mailbox list, click the mailbox name that you would like to forward.

   <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-6.png %}" />

9. Click the **Mail Forwarding** tab. On the Mail Forwarding screen, select **Forward to an Exchange address within this domain**.

    **Note:** Forwarding to an Exchange address within another domain on this account will work only if both domains are on the same Exchange server. If you are not sure if both domains are on the same Exchange server, create a contact for the domain you want to forward to.

10. Select the Distribution List address you just created.

11. Select the **Save copies of forwarded email** option.

    <img src="{% asset_path exchange/set-up-microsoft-exchange-email-forwarding/hex-forward-multi-7.png %}" />

    If **Save a copy of forwarded email** is not checked, this mailbox _not_ store any messages sent to it.

11. Click **Save**. Allow at least 15 minutes for the forward to enable.

### References

- [Cloud Office Control Panel](https://cp.rackspace.com/)
- [Cloud Office support terminology](/how-to/cloud-office-support-terminology)
- [Cloud Office Email Portal](https://apps.rackspace.com/index.php)
- [Set up Rackspace Email forwarding](/how-to/set-up-rackspace-email-forwarding/)