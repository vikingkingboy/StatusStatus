# Project Name / Hosting Setup Guide

Brief description of your project or website.  
Example: This is a simple portfolio site / business landing page / WordPress blog hosted on cPanel.

**Important requirement**  
You **must** have a **cPanel hosting account** with email support enabled (most shared hosting providers include this by default).

## Prerequisites

- A domain name pointed to your cPanel hosting (A record / nameservers set up)
- Access to cPanel (usually https://yourdomain.com/cpanel or https://server-ip:2083)
- cPanel username and password from your hosting provider

## Step 1: Log in to cPanel

1. Go to your hosting provider's client area and find the "Login to cPanel" button,  
   or directly visit:  
   `https://yourdomain.com/cpanel` or `https://serverhostname:2083`
2. Enter your cPanel username and password.

## Step 2: Create a Functional Email Account

cPanel makes it very easy to create professional email addresses like name@yourdomain.com.

1. In cPanel, scroll to the **Email** section.
2. Click on **Email Accounts**.
3. Click the **+ Create** / **Create** button (usually in the top right).
4. Fill in the details:
   - **Domain**: Select your domain from the dropdown (if you have multiple).
   - **Username**: Enter the part before the @ (e.g. info, support, yourname).
   - **Password**: Enter a strong password (or click **Generate** for a secure one — copy it!).
   - **Mailbox Quota**: Set to "Unlimited" or a reasonable size (e.g. 1–10 GB).
5. Click **+ Create** / **Create Account**.
6. Wait a few seconds — the account is now created!

## Step 3: Access Your New Email (Webmail)

The fastest way to check if the email works:

1. Back in the **Email Accounts** list, find your new email.
2. Click **Check Email** or **Webmail** next to it.
3. Choose a webmail client (Roundcube or Horde are common and work great).
4. Log in with your full email address and the password you set.
5. Send a test email to yourself or another address (e.g. your Gmail) to confirm it's working both ways.

## Step 4: (Optional) Set Up Email on Your Phone or Computer

1. In the **Email Accounts** list, click **Connect Devices** or **Set Up Mail Client** next to your email.
2. cPanel shows ready-to-use settings:
   - **Incoming Server**: Usually mail.yourdomain.com (IMAP port 993 SSL or POP3 995 SSL)
   - **Outgoing Server**: mail.yourdomain.com (SMTP port 465 SSL or 587 TLS)
   - Username: your full email address
   - Password: the one you created
3. Use these in Outlook, Thunderbird, Apple Mail, Gmail app, iPhone Settings → Mail, Android Email app, etc.

## Troubleshooting Tips

- **Email not sending/receiving?**  
  → Check SPF, DKIM, DMARC records in cPanel → **Email** → **Email Authentication** (enable them — highly recommended).  
  → Make sure your domain's MX records point to your cPanel server (check in **Zone Editor**).
- **Login issues?** → Double-check password (case-sensitive). Reset via **Email Accounts** → **Manage**.
- **Spam in inbox?** → Use filters or enable SpamAssassin in cPanel.

## Contact / Support

If you run into hosting-specific issues, contact your hosting provider's support (they usually have 24/7 chat/tickets).

For project-related questions: [your contact info / GitHub issues / email]

---

Last updated: February 2026  
Made with ❤️ for anyone setting up email on cPanel.
