---
summary: Explore how to stream logs from OutSystems 11 (O11) applications to Elastic APM by configuring LifeTime with the necessary credentials.
tags: log management, application monitoring, elastic stack, performance analysis, observability
locale: en-us
guid: 1b3c1db5-f89c-4ec8-a921-d91cbff3a4ea
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma:
audience:
  - platform administrators
  - backend developers
  - full stack developers
  - tech leads
  - infrastructure managers
outsystems-tools:
  - lifetime
  - platform server
coverage-type:
  - apply
---

# Stream logs to Elastic 

This article explains how you can set up log streaming from OutSystems applications to the **Elastic** APM tool. 

## Prerequisites

Before streaming logs to Elastic, ensure you have: 

* Enabled [Log separation](../../setup-infra-platform/setup/logging-db/logs-separation-cloud/intro.md). 

* Installed Platform Server version 11.23.1 or higher (recommended Platform Server version is 11.30.0 or higher).

* Installed LifeTime version 11.19.0 or higher (recommended LifeTime version is 11.25.0 or higher).

* Have subscription to log streaming. Contact your Account Manager for provisioning.

## Set up log streaming

<div class="info" markdown="1">

* Native Elastic APM OpenTelemetry log ingestion is only available in version 8.0 onwards.

* The Elastic Observability services and Kibana plugins must be deployed alongside the Elasticsearch cluster to complete the following steps.

</div>

To set up the log streaming to Elastic, you need the **Elastic URL** and **Secret token** values. Once you have these, go to LifeTime and [configure the log streaming service](lifetime-streaming.md).

## Additional resources

* [Elastic Observability](https://www.elastic.co/observability)

* [OpenTelemetry integration in Elastic](https://www.elastic.co/guide/en/apm/guide/8.6/open-telemetry.html) 

* [OpenTelemetry Collector configuration](https://opentelemetry.io/docs/collector/configuration/)

