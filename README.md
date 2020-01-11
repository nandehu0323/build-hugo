# Build Hugo

A GitHub Action to build Hugo site.

- Using [Hugo extended version 0.62.2](https://github.com/gohugoio/hugo/releases/tag/v0.62.2)
- Using [debian:buster-slim](https://hub.docker.com/_/debian/) as the base image

Example workflow

```
name: Build Hugo
on: [push]
jobs:
  build:
    name: Build
    runs-on: ubuntu-latest
    steps:
    - name: Check out code
      uses: actions/checkout@master
    - name: Build Hugo
      uses: nandheu0323/build-hugo@v0.62.2
```
