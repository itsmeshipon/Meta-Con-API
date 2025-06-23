Important Code for GTM — Facebook Pixel Conversion API
This repository contains essential scripts and helper snippets to implement and manage Facebook Pixel Conversion API using Google Tag Manager (GTM).

📌 Purpose
Improve Facebook Pixel data quality by sending server-side events.

Reduce data loss due to browser restrictions (e.g., iOS tracking limits, ad blockers).

Maintain accurate tracking for better campaign optimization and reporting.

📂 What’s Inside
Event Matching Helpers: Scripts to collect user parameters (e.g., email, phone) and pass them securely.

Custom HTML Tags: Ready-to-use code snippets to send server events via your chosen server endpoint.

Data Layer Examples: Templates to push event data and user identifiers.

Debugging Tools: Helper scripts to test events and verify server responses.

⚙️ How to Use
Clone or download this repository.

Select the script you need for your GTM setup.

Add the code in a Custom HTML Tag in GTM.

Configure triggers based on your website’s conversion actions.

Connect GTM to your server endpoint (e.g., using a server container or third-party service like Stape).

Test events with Facebook’s Event Manager and Test Events Tool.

✅ Best Practices
Always hash user data before sending.

Test thoroughly in GTM Preview mode.

Keep your server endpoint secure and monitor for errors.

Follow Facebook’s guidelines for Event ID usage to prevent duplication.

🤝 Contributing
Have improvements or additional scripts? Feel free to fork this repository, add your code, and submit a pull request.
