---
title: "Cloud Monitoring CLI"
draft: false
date: 2021-02-14
tags: ["monitoring","stackdriver","cli"]
searchHidden: false

---

gmon is a command-line interface for Cloud Monitoring written in Python.

The CLI supports the following endpoints:

metrics (GA): Manage Cloud Monitoring metrics.
accounts (EAP): Manage Cloud Monitoring accounts.
services (ALPHA): Manage Cloud Monitoring services.
slos (ALPHA): Manage Cloud Monitoring service level objectives.
Other endpoints are available directly in gcloud alpha monitoring, and won't be added to gmon, in particular:

channel-descriptors: (ALPHA) Cloud Monitoring notification channel descriptors.
channels: (ALPHA) Manage Cloud Monitoring notification channels.
policies (ALPHA): Manage Cloud Monitoring alerting policies.
dashboards (GA): Manage Cloud Monitoring dashboards.
The goal of this CLI is to fill the gap and simplify users life to query monitoring endpoints in a more friendly manner and troubleshoot their monitoring setups.



Link: https://github.com/GoogleCloudPlatform/professional-services/tree/main/tools/gmon