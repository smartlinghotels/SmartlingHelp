---
title: Reduce time to market with Pre-Publish
layout: blogpost
banner_image: /uploads/smartling---translation-workflow--smartling-hotels-.png
blog-author: Andrew Saxe
categories:
  - tips
---


Smartling offers a Workflow option to make content live - on a Web site, in a CMS, in a file - without taking it out of the workflow. &nbsp;We call this Pre-Publish. &nbsp;With our just released feature of Pre-Publish on Save, this is another option to accelerate pushing content live.

Pre-Publish is especially useful for customers using GDN and for customers who have integrated into the API with a callback URL.

## Global Delivery Network (GDN)

Whenever content is Saved or Submitted and Pre-Publish is ON, translations are pushed to the live language web site immediately. &nbsp;The content will continue through the Workflow and update at each following Workflow Step.

![](/uploads/versions/image00---x----677-292x---.png)

## File API with Callback or CMS Connectors

If a customer has integrated with the Smartling File API and has passed a callback URL, as content is completed - a string or an entire file - Smartling will execute a callback to whatever URL was passed in with the string or file on initial upload. &nbsp;This gives the opportunity to validate in-progress translations or push translations live immediately. &nbsp;The content will continue through the Workflow and update at each following Workflow Step.

![](/uploads/versions/image01---x----647-301x---.png)