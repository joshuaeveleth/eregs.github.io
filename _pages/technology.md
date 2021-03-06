---
layout: default
title: Technology
subtemplates: [architecture, stack, repos]
---
# Code and documentation


**Table of contents**

* [How eRegulations works](#how-eregulations-works)
* [Repositories](#repositories)
  * [The main body of eRegulations (not agency-specific)](#main-repositories)
  * [Agency-centric components](#agency-repositories)
* [Open source and contributing](#open-source-and-contributing)

## How eRegulations works

{% for subtemplate in page.subtemplates %}
  {% capture subtemplate_file %}technology/{{subtemplate}}.md{% endcapture %}
  {% capture markdown %}{% include {{subtemplate_file}} %}{% endcapture %}
  {{ markdown | markdownify }}
{% endfor %}

## Open source and contributing

We invite contributions to any part of the application, from people inside and outside government. The project is in the public domain, and all contributions to it will be released as such. By submitting a pull request, you are agreeing to waive all rights to your contribution under the terms of the [CC0 Public Domain Dedication](http://creativecommons.org/publicdomain/zero/1.0/).

If you contribute the open source work of others, please mark it clearly in your pull request.