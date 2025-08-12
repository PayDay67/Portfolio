# Formspree Setup - Get Your Own Form Endpoint

The current form uses a temporary endpoint. To receive emails in your Gmail (princevikram7267@gmail.com):

## Steps:
1. Go to https://formspree.io/
2. Sign up with your email
3. Create a new form
4. Enter your email: princevikram7267@gmail.com
5. Copy your form endpoint (looks like: https://formspree.io/f/YOUR_FORM_ID)
6. Replace "xpwaqjko" in both index.html and contact.html with your actual form ID

## Current form action:
```html
<form action="https://formspree.io/f/xpwaqjko" method="POST">
```

## Replace with your endpoint:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

After setup, you'll receive all form submissions directly in your Gmail!