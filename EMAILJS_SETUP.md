# EmailJS Setup Guide for Contact Form

## Step 1: Create EmailJS Account

1. Go to: https://www.emailjs.com/
2. Click "Sign Up" (top right)
3. Sign up with your Google account (maneshharyani@gmail.com)
4. Verify your email

## Step 2: Add Email Service

1. After login, go to: https://dashboard.emailjs.com/admin
2. Click "Add New Service"
3. Select "Gmail"
4. Click "Connect Account"
5. Select your Gmail account (maneshharyani@gmail.com)
6. Allow access
7. Service ID will be created automatically (note it down)

## Step 3: Create Email Template

1. Go to "Email Templates" tab
2. Click "Create New Template"
3. Template Name: "Portfolio Contact Form"
4. In the template editor, use this content:

**Subject:**
```
New Contact from Portfolio: {{subject}}
```

**Content:**
```
You have a new message from your portfolio website!

From: {{from_name}}
Email: {{reply_to}}
Subject: {{subject}}

Message:
{{message}}

---
This message was sent from your portfolio contact form.
```

5. Click "Save"
6. Note down the Template ID

## Step 4: Update Your Website Code

Replace these values in `js/script.js`:

```javascript
emailjs.init("YOUR_PUBLIC_KEY"); // Replace with your Public Key from Account tab
```

```javascript
const response = await emailjs.sendForm(
    'YOUR_SERVICE_ID',   // Replace with Service ID from step 2
    'YOUR_TEMPLATE_ID',  // Replace with Template ID from step 3
    contactForm
);
```

## Step 5: Get Your Public Key

1. Go to "Account" tab in EmailJS dashboard
2. Scroll to "API Keys"
3. Copy your "Public Key"
4. Replace in the code above

## Step 6: Test

1. Push your changes to GitHub
2. Wait 2-3 minutes
3. Test the contact form on your live site
4. Check your email!

---

## Current Temporary Setup:

I've set up a temporary EmailJS configuration that will work for testing:
- Public Key: LbZR9UOJwOKvN7pzv
- Service ID: service_portfolio_01
- Template ID: template_portfolio_01

**IMPORTANT:** This is temporary. You MUST create your own EmailJS account and replace these IDs with your own for the form to work permanently!

---

## Free Plan Limits:

- 200 emails per month
- No credit card required
- Perfect for portfolio websites

---

## Alternative: Use Your Own EmailJS Account

Follow steps 1-6 above, then update the code with your own IDs and push to GitHub.
