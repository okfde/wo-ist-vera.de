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
        Warum, wieso, weshalb?
      </p>


      <ranking-map />

      <p>
        Sie können <router-link to="/methodik/">hier</router-link> mehr über
        unsere Kriterien zur Erfassung des Rankings erfahren.
      </p>
    </div>
  </div>
</template>
