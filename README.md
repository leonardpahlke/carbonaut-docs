# Carbonaut Documentation Website

Documentation for the [Carbonaut project](https://github.com/leonardpahlke/carbonaut)

## Local Development

Pre-requisites: [Hugo](https://gohugo.io/getting-started/installing/), [Go](https://golang.org/doc/install) and [Git](https://git-scm.com)

```shell
# Clone the repo
git clone https://github.com/leonardpahlke/carbonaut-docs.git

# Change directory
cd carbonaut-docs/

# Start the server
hugo mod tidy
hugo server --logLevel debug --disableFastRender -p 1313
```

## Update theme

```shell
hugo mod get -u
hugo mod tidy
```

See [Update modules](https://gohugo.io/hugo-modules/use-modules/#update-modules) for more details.

