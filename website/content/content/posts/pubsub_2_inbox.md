---
title: "Pubsub2Inbox- PubSub to Email/Webhook/GCS"
draft: false
date: 2021-02-14
tags: ["pubsub","billing","alert","notification"]
searchHidden: false

---

Pubsub2Inbox is a generic tool to handle input from Pub/Sub messages and turn them into email, webhooks or GCS objects. It's based on an extendable framework consisting of input and output processors. Input processors can enrich the incoming messages with details (for example, fetching the budget from Cloud Billing Budgets API). Multiple output processors can be chained together.

Pubsub2Inbox is written in Python 3 and can be deployed as a Cloud Function easily. To guard credentials and other sensitive information, the tool can fetch its YAML configuration from Google Cloud Secret Manager.

The tool also supports templating of emails, messages and other parameters through Jinja2 templating.

Link: https://github.com/GoogleCloudPlatform/professional-services/tree/main/tools/pubsub2inbox