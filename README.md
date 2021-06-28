# Wo-ist-VERA.de

[![Build status](https://github.com/okfde/wo-ist-vera.de/actions/workflows/build.yml/badge.svg)](https://github.com/okfde/wo-ist-vera.de/actions/workflows/build.yml)

[wo-ist-vera.de](https://wo-ist-vera.de) macht den Umgang aller Bundesländer mit VERgleichsArbeiten transparent.

## Setup

```bash
yarn install
yarn dev # start dev server
yarn build # build for production
```

## Content

Der Inhalt der Seite wird aus den YAML- und Markdowndateien unter
[`./src/data`](./src/data) generiert.

### Kategorien und Kriterien

Die [Kategorien](./src/data/categories.yml) bestehen aus `title`, `slug` (ein
URL-freundlicher, einmaliger Identifier), `color` (einer CSS-kompatiblen Farbe,
etwa `#fff`) und einer `description`.

Zu diesen Oberkategorien können die [Rankingkriterien](./src/data/criteria.yml)
angelegt werden. Diese bestehen ebenfalls aus `title` und `description`,
beinhalten zudem auch die Eigenschaft `maxPoints` (der für dieses Kriterium
maximal erreichbaren Punktzahl). Die übergeordnete Kategorie kann mit `category`
gesetzt werden. Dabei wird der `slug` einer aus der
[Kategoriedatei](./src/data/categories.yml) angegeben.

### Länder

Jedes Land hat unter [`./src/data/states`](./src/data/states) sowohl eine
gleichnamige Markdown- und YAML-Datei (etwa `berlin.md` und `berlin.yml`). Zudem
sollte unter [`./src/assets/img/wappen`](./src/assets/img/wappen) ein Wappen im
svg-Format abgelegt werden (ebenfalls gleicher Dateiname). In der Markdowndatei
kann eine ausführliche Beschreibung zum Land formuliert werden.

## Lizenz

Der Code ist [MIT-lizensiert](./LICENSE), die Inhalte (alle `.yml` und `.md`
sowie `.csv` Dateien) fallen unter [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).


