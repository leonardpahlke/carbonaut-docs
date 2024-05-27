---
title: How to Run Carbonaut
weight: 1
slug: how-to-run
---

Carbonaut can be run as binary or container. The latest releases can be found [here](https://github.com/leonardpahlke/carbonaut/releases).


{{% steps %}}

### Download the Binary

1. **Binary**: navigate to [Carbonauts releases page](https://github.com/leonardpahlke/carbonaut/releases) and pull the version for your machine
2. **Container**: **TBD**

### Create a configuration file

In order to tell which plugins Carbonaut should load and where to find your resources, Carbonaut requires a configuration file. The file is passed on start with the `-c` flag. See [configuration reference](/docs/reference/configuration/) for more information how to setup the config file.

### Run Carbonaut

1. **Binary**: `carbonaut -c config.yaml` will start Carbonaut. The configuration can be updated during runtime (see [Server API](/docs/reference/server-api/))
2. **Container**: **TBD**

{{% /steps %}}
