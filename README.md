# Wo-ist-VERA.de

[![Build status](https://github.com/okfde/wo-ist-vera.de/actions/workflows/build.yml/badge.svg)](https://github.com/okfde/wo-ist-vera.de/actions/workflows/build.yml)

[wo-ist-vera.de](https://wo-ist-vera.de) macht den Umgang aller Bundesländer mit VERgleichsArbeiten transparent. Die Plattform ist ein Fork von [transparenzranking.de](https://transparenzranking.de/).

## Setup

```bash
yarn install
yarn dev # start dev server
yarn build # build for production
```

## Content

Der Inhalt der Seite wird aus den YAML- und Markdowndateien unter
[`./src/data`](./src/data) generiert.

## Lizenz

Der Code ist [MIT-lizensiert](./LICENSE), die Inhalte (alle `.yml` und `.md`
sowie `.csv` Dateien) fallen unter [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).


