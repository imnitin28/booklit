# booklit

[![Go Reference](https://pkg.go.dev/badge/github.com/vito/booklit.svg)](https://pkg.go.dev/github.com/vito/booklit)
[![CI](https://ci.concourse-ci.org/api/v1/teams/main/pipelines/booklit/jobs/unit/badge)](https://ci.concourse-ci.org/teams/main/pipelines/booklit/jobs/unit)

## documentation

[vito.github.io/booklit](https://vito.github.io/booklit)

## installation

grab the latest [release](https://github.com/vito/booklit/releases), or build
from source:

```bash
go get github.com/vito/booklit/cmd/booklit
```

## usage

```bash
booklit -i foo.lit -o ./out
```

## example

clone this repo and build its docs:

```bash
booklit \
  -i docs/lit/index.lit \
  -o docs \
  --html-templates docs/lit/html \
  --plugin github.com/vito/booklit/booklitdoc \
  --plugin github.com/vito/booklit/chroma/plugin
```

then browse the generated docs from `./docs/index.html`.

you can see the result at https://vito.github.io/booklit
