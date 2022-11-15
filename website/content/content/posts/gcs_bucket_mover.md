---
title: "GCS Bucket Mover Tool"
draft: false
date: 2021-02-14
tags: ["gcs","bucket","transfer","google-cloud-storage"]
searchHidden: false

---
Currently there is no built in way to move a GCS bucket and all objects from one project to another. The manual process is:

* Note down all settings related to the source bucket
* Create a temporary bucket in the target project
* Create a Storage Transfer Service (STS) job to move all objects from the source bucket to the temporary bucket
* Delete the source bucket
* Immediately re-create the bucket in the target project
* Create an STS job to move all objects from the temporary bucket to the new source bucket in the target project
* Delete the temporary bucket
* Re-apply all bucket settings from the source bucket
This tool is designed to automatically perform these steps to make a bucket move as seamless as possible.

Link: https://github.com/GoogleCloudPlatform/professional-services/tree/main/tools/gcs-bucket-mover