---
title: Build Carbonaut Manually
weight: 6
slug: how-to-build
---

The project pushes binaries to the GitHub release and Docker containers can be build locally. If you prefer to build binaries manually, you can follow these instructions. In general the entire build process pushing to GitHub is part of the Carbonaut repository.

{{% steps %}}

### Prerequisits install project dependencies

Setup your dev environment. Follow this [guide](/docs/guides/how-to-setup-dev-environment/).

### Build Go Binaries

Binaries are automatically created if there is a new tag created in the Carbonaut repository. The project uses [goreleaser](https://goreleaser.com/) to manage the automation - see [release workflow](https://github.com/leonardpahlke/carbonaut/blob/main/.github/workflows/release.yml). These binaries are getting added to the release page - see [releases](https://github.com/leonardpahlke/carbonaut/releases).

Binaries can be created manually via `go build`

### Build Container Images

Container images are created using [Ko](https://ko.build/). To build container images locally run `make container-build-local`. Currently container images are not pushed to a public container registry.

{{% /steps %}}
