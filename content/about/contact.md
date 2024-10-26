---
# An instance of the Contact widget.
# Documentation: https://docs.hugoblox.com/getting-started/page-builder/
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 50

title: Get in touch
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: true

  # Email form
  form:
    action: "https://api.staticforms.xyz/submit"
    method: "post"
    fields:
      - name: "name"
        type: "text"
        placeholder: "Your Name"
      - name: "email"
        type: "email"
        placeholder: "Your Email"
      - name: "message"
        type: "textarea"
        placeholder: "Your Message"
      - name: "honeypot"
        type: "text"
        style: "display:none"
      - name: "accessKey"
        type: "hidden"
        value: "your-access-key"  # Replace with your actual access key
      - name: "subject"
        type: "hidden"
        value: "Contact us from - example.com"  # Adjust as needed
      - name: "replyTo"
        type: "hidden"
        value: "@"
      - name: "redirectTo"
        type: "hidden"
        value: "https://example.com/contact/success"  # Redirect URL after submission

design:
  columns: '1'
---
