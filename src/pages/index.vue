<template>
  <div class="container flex flex-col items-center">
    <h1 class="headline">Transparenz für Vergleichsarbeiten</h1>

    <div class="prose prose-lg text-center">
      <p class="max-w-screen-lg w-full text-center">
        VERA - VERgleichsArbeiten - sind standardisierte Kompetenzerhebungen, die länderübergreifend Lernstände festhalten. Mit ihnen lässt sich der Erfolg bildungspolitischer Maßnahmen bestimmen. Doch sie stehen weitestgehend unter Verschluss. Wir machen sichtbar, welche Bundesländer blockieren und wo nachzubessern ist. Außerdem veröffentlichen wir die vorhandenen Daten in maschinenlesbarer Form.
      </p>
    </div>

    <ranking-overview class="my-12" />

    <div class="prose prose-lg">
      <p>
        In Deutschland wird Bildungspolitik in einer Blackbox gemacht. Es gibt kaum Nationen, die so wenig über ihr Schulsystem wissen, wie Deutschland. Und die wenigen Daten, die vorliegen, halten die Bundesländer weitestgehend unter Verschluss. Wie problematisch das ist, zeigt sich gerade besonders: Alle reden über pandemiebedingte Lernrückstände, aber inwiefern die genau existieren, weiß niemand so genau - weil die Daten nicht vorliegen. Wie sollen so effektive Maßnahmen ergriffen werden?
      </p>
      <p>
        Dabei werden Daten erhoben und das schon seit Jahren. Die sogenannten VERgleichsArbeiten (kurz VERA) sind weitestgehend standardisierte Kompetenztests. Mit ihnen werden Grundkompetenzen erhoben, wie Lesefähigkeit, Schreibfähigkeit oder mathematische Grundkenntnisse. Auf Wo-ist-VERA.de veröffentlichen wir zum ersten Mal vorhandene Daten an einem zentralen Ort. Außerdem vergleichen wir den Umgang der Bundesländer mit VERA.
      </p>


      <ranking-map />

      <p>
        Sie können <router-link to="/methodik/">hier</router-link> mehr über
        unsere Kriterien zur Erfassung des Rankings erfahren.
      </p>
    </div>
  </div>
</template>
