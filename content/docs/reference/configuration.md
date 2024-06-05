---
title: Configuration
slug: configuration
weight: 3
---

Carbonaut has example configurations pushed to the repository (see [examples](https://github.com/leonardpahlke/carbonaut/tree/main/example)).

```yaml
kind: carbonaut
meta:
    name: carbonaut
    log_level: info
    connector:
        timeout_seconds: 10
spec:
    provider:
        resources:
            equinix:
                static_resource:
                    plugin: equinix
                    access_key_env: "METAL_AUTH_TOKEN"
                dynamic_resource:
                    plugin: scaphandre
                    endpoint: ":8080/metrics"
        environment:
            dynamic_environment:
                plugin: electricitymaps
                access_key_env: "ELECTRICITY_MAP_AUTH_TOKEN"
    server:
        port: 8088

```