# action-repo
test pull
This repo is used to send GitHub activity (like push, pull request, or merge) to a server using webhooks.

What It Does
Whenever someone:

pushes code

creates or merges a pull request

GitHub will send that info to your server using a webhook.

How to Set Up Webhook
Go to Settings → Webhooks in your GitHub repo

Click Add webhook

Fill in:

Payload URL: http://<your-server-ip>:5000/webhook
Example my payload url is  https://5cb4-2405-201-31-b89a-d512-66fa-2927-87f8.ngrok-free.app

Content type: application/json

Choose events (push, pull request, etc.)

Click Add webhook

What You Need on Server
Flask app (app.py) to receive events

models.py to save data in MongoDB

index.html to show events on a webpage

Result
You’ll see GitHub events live on your webpage with time and type (push, pull request, or merge).

