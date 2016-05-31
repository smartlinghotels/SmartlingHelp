---
layout: article
title: Integrate Machine Translation Into A Workflow
draft: true
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
    - section
  articles:
    - article
  others:
    - link:
      text:
further-reading:
  include: false
  sections:
    - section
  articles:
    - article
  others:
    - link:
      text:
migration-checklist:
  internal-links: false
  images: false
  FAQs: false
  related: false
---
Smartling allows you to seamlessly integrate translation work from an external provider, such as a Machine Translation service, into your Smartling workflow. Content you authorize in Smartling will be sent to the external provider for translation and submitted to the next step in your workflow when Translation is complete.

Third Party providers must register with Smartling before they can be integrated into an external step. Currently registered third party providers are:

*   [Google Translate](/hc/en-us/articles/203237753)
*   Unbabel
*   CrossLang
*   Microsoft Bing

Third-Party machine translations will only be applied to untranslated strings. Machine translation from an External Workflow Step will not overwrite existing translations.

**Note:** Timeframes and payment are negotiated between the client and the Third Party provider. Smartling cannot guarantee timeframe or quality of translations from a Third Party provider.

**To set up an External Workflow Step:**

**(1)** From **Project Settings > Translation Workflow**, edit the Translation step of the workflow you want translated by an external provider.

****![](/hc/en-us/article_attachments/205411447/Smartling___Translation_Workflow.png)****

**(2)** Select your provider from the drop-down list and fill in the required detail fields. These fields are set by the provider and are used to identify you for authentication and billing purposes. Possible fields might include a username, password, API Key, etc. If you are unsure of how to complete the required fields, contact the external provider.



Once your External Workflow Step is set up, any authorized content will be sent to the provider. After translation it will be submitted to the next step in your workflow. For example, if you have an Edit step next, the appropriate translation resources will be receive a notification that content is available for editing. If the next step in your workflow is Published, content will be published as soon as it is received from the external provider.

****Note:** Some third party providers may restrict the rate at which content is translated. If a string has been sent to a third party provider and no translation has been received, it will display an **In Queue** >notice in the List View.**