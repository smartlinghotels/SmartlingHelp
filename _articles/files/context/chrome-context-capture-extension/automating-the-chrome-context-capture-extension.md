---
layout: article
title: Chrome Context Capture Extension - Automation
draft: false
Applies to:
  GDN: false
  Application-Resource-Files: false
  CMS-Connectors: false
redirect-url:
wistia:
  video: false
  id:
read-first:
  include: false
  sections:
  articles:
  others:
    - link:
      text:
further-reading:
  include: false
  sections:
  articles:
  others:
    - link:
      text:
migration-checklist:
  internal-links: true
  images: false
  FAQs: false
  related: false
  reviewed: false
---


The Chrome Context Capture Extension can be automated to capture context for an entire website. The Automation Tool is only available for Application Resource Files projects.

By default the Chrome Context Capture Extension will not override existing context.

**1)** In Chrome, navigate to **Chrome&gt;Preferences&gt;Extensions** and click **Options**.

![](/uploads/versions/extensions-2---x----918-428x---.png)

**2)** Select **Automation Tool**

![medium](/uploads/versions/smartling_context_snapshot_options-1---x----688-752x---.png)

**3)** Drag your site’s sitemap.xml file into the marked area.

![](/uploads/versions/smartling_context_snapshot_options-2---x----1247-141x---.png)

In your sitemap.xml file you can create a `<url-list>` node populated with a list of URLs you wish to contextualize. You can also preload your Project UID and API key by adding this code at the top of your sitemap:

~~~
<smartlingconfig>
    <apikey>#######</apikey>
    <projectUID>#######</projectUID>
</smartlingconfig>
~~~

You can download a custom sitemap template [here](/public/smartling-chrome-automation-sitemap-example.xml)

**4)** Set up the automation tool:

![](/uploads/versions/smartling_context_snapshot_options-3---x----946-525x---.png)

* **Project UID** - Can be found on the Dashboard at **Project Settings > API**.
* **API Key** - Can be found on the Dashboard at **Project Settings > API**.
* **Wait** - Instructs the Chrome Context Capture Extension to wait X milliseconds after loading a page to take a snapshot. Use this feature if you have javascript that executes on loading a page.
* **Advanced** - allows you to execute custom javascript on each page before taking a snapshot.
* **URL Filter** - Filters URLs by text. Snapshots will only be taken of URLs matching your filter text.
* **Test mode** - If checked, the Chrome Context Capture Extension will crawl the selected urls, but will not take snapshots. You can also click test next to any URL to view a preview snapshot for that URL.


**5)** Click **Start**. The Automation Tool will capture a snapshot of each selected URL and match the snapshots to any matching strings in your project.