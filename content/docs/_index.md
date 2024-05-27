---
title: Documentation
next: first-page
---


![carbonaut banner image](carbonaut-banner.png)

Carbonaut is project to collect and refine environmental sustainability data from your IT infrastructure and make it available in a common data schema. The project does not implement a scraper to scan your IT infrastructure or measure your virtual machine energy, but integrates over providers which are implemented as plugins to integrate external data sources. The project is a POC and therefore not production ready. If you like to [contribute](/docs/reference/contributing) you are very welcome to do so!

{{< callout type="warning" >}}
  Carbonaut is a proof of concept project which may be turned in the future into a proper open source project. Right now this is not the case.
{{< /callout >}}

The aim of the project is to collect and integrate data around environmental sustainability and make it accessible to users so that they can make automatic or manual decisions. The project integrates heterogenous data sources over plugins and transforms the data in a simple minimalistic data schema. Carbonaut discovers created IT infrastructure, maintains a minimalistic internal static resource state and chains dynamic changing data together to collect a holistic overview of cloud native sustainability data.

![carbonaut context](/concepts/context.drawio.png)


{{< cards >}}
  {{< card link="guides/how-to-run" title="Running Carbonaut" icon="book-open" >}}
  {{< card link="components" title="Carbonaut Internal Components" icon="document-text" >}}
  {{< card link="contributing" title="Carbonaut Contributor Guide" icon="users" >}}
  {{< card link="reference" title="Carbonaut References" icon="cog" >}}
{{< /cards >}}
