# NW build action

GitHub action for building applications based on NW framework. See
[nw-build](https://google.com/).

## Getting started

Here's an example that builds NW XML editor (a simple test application on NW
framework):

    name: build nw-xml-editor
    on: push
    jobs:
      build:
        runs-on: windows-latest
        steps:
          - name: Build nw-xml-editor
            uses: sphericalpm/nw-build-action@v1
            with:
              app: nw-xml-editor
