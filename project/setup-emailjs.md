# EmailJS Setup Instructions

To receive emails directly in your Gmail (princevikram7267@gmail.com), follow these steps:

## 1. Create EmailJS Account
- Go to https://www.emailjs.com/
- Sign up with your email
- Verify your email address

## 2. Add Email Service
- Go to Email Services
- Click "Add New Service"
- Choose "Gmail"
- Connect your Gmail account (princevikram7267@gmail.com)
- Note the Service ID (e.g., "service_abc123")

## 3. Create Email Template
- Go to Email Templates
- Click "Create New Template"
- Use this template:

```
Subject: {{subject}}

New message from your portfolio website:

Name: {{from_name}}
Email: {{from_email}}

Message:
{{message}}
```

- Note the Template ID (e.g., "template_xyz789")

## 4. Get Public Key
- Go to Account > General
- Copy your Public Key (e.g., "user_abcdef123456")

## 5. Update script.js
Replace these placeholders in script.js:
- `YOUR_PUBLIC_KEY` with your actual public key
- `YOUR_SERVICE_ID` with your Gmail service ID
- `YOUR_TEMPLATE_ID` with your template ID

## Example:
```javascript
emailjs.init('user_abcdef123456');

emailjs.send('service_abc123', 'template_xyz789', {
    // ... rest of the code
```

After setup, visitors can send messages directly to your Gmail!