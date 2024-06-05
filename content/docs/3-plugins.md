---
title: Plugins
weight: 5
slug: plugins
---

Carbonaut Plugin information. Implementations are located in the [`pkg/plugins`](https://github.com/leonardpahlke/carbonaut/tree/main/pkg/plugin) folder.

### Dynamic Environment Plugins

[Electricity Map](https://www.electricitymaps.com) plugin implementation.

* Configuration key: `electricitymaps`
* Requires an API key which is specified as environment variable in the carbonaut configuration file. 

**Example configuration**:
```yaml
dynamic_environment:
    plugin: electricitymaps
    access_key_env: "ELECTRICITY_MAP_AUTH_TOKEN"
```

### Dynamic Resource Plugins

[Scaphandre](https://github.com/hubblo-org/scaphandre) plugin implementation.

* Configuration key: `scaphandre`
* Requires information about the port and endpoint 

**Example configuration**:
```yaml
dynamic_resource:
    plugin: scaphandre
    endpoint: ":8080/metrics"
```

### Static Resource Plugins

[Equinix](https://www.equinix.com/) plugin implementation.

* Configuration key: `equinix`
* Requires an API key which is specified as environment variable in the carbonaut configuration file. 

**Example configuration**:
```yaml
xyz-equinix-abc:
    static_resource:
        plugin: equinix
        access_key_env: "METAL_AUTH_TOKEN"
```
