<template>
  <div class="container">
    <h1 class="mb-0 headline">Wie sollten die VERA-Daten veröffentlicht werden?</h1>

    <div class="prose prose-lg mt-4">
      <h2>Unsere Kriterien</h2>

      <p>
        Bei der Punktevergabe wird die Transparenzbereitschaft am stärksten belohnt (Transparenz der Daten). Bundesländer, die selbstständig Daten veröffentlichen, haben also automatisch zwei Punkte mehr, als solche, die es nur auf Anfrage machen, aber möglicherweise umfänglichere Daten zur Verfügung stellen. Viele Punkt können die Bundesländer auch durch die Veröffentlichung der jährlichen VERA-Ergbenisse sammeln (Vollständigkeit der Daten). Besonders belohnt wird auch die Auflösung der Ergebnisse über die Landesebene hinaus (Auflösung der Daten).
      </p>

      <p>
        Gemeinsam ergeben die Bewertungen für die verschiedenen Bereiche die
        mögliche Höchstpunktzahl von 100 Prozent.
      </p>

      <methodology-heading :category="getCategory('qualitaet')" />

      <p>
        Es ist intransparent, dass einige Bundesländer die Daten nur auf Anfrage herausgeben. Um mit den Daten arbeiten zu können ist es notwendig, dass sie in maschinenlesbarer Form vorhanden sind. Das ist leider selten der Fall. In der Regel müssen sie aufwändig aus PDF-Dateien, Briefen oder E-Mails extrahiert und strukturiert werden. Darum erhalten die Länder mehr Punkte, die selbstständig und maschinenlesbar veröffentlichen. Die Maximalpunktzahl ist 4.
        <ul>
            <li>selbstständig und maschinenlesbar veröffentlicht (4 Punkte)</li>
            <li>selbstständig, aber nicht maschinenlesbar veröffentlicht (3 Punkte)</li>
            <li>nur auf Anfrage, aber maschinenlesbar veröffentlicht (2 Punkte)</li>
            <li>nur auf Anfrage und nicht maschinenlesbar veröffentlicht (1 Punkt)</li>
        </ul>
      </p>
      <methodology-heading :category="getCategory('vollstaendigkeit')" />
      <p>
        Die Bundesländer haben sich seit dem Schuljahr 2008/09 darauf geeinigt, weitestgehend standardisiert Vergleichsarbeiten durchzuführen. Wenige Bundesländer haben damit bereits früher begonnen. Aus diesem Grund beschränkt sich das Ranking auf den Zeitraum 2008/09 bis 2019/20. Für jedes Jahr, aus dem Daten verfügbar sind, gibt es einen Punkt. Die Maximalpunktzahl liegt also bei 12. Denn um Aussagen über bildungspolitische Maßnahmen und ihre Wirkung treffen zu können, braucht es regelmäßige Erhebungen, um die Daten Maßnahmen sinnvoll zuordnen zu können.
      </p>

      <methodology-heading :category="getCategory('aufloesung')" />
      <p>
        Je kleinräumiger Bildungsdaten verfügbar sind, desto flexibler und genauer können Fähigkeiten von Lernenden beschrieben, Wirkungsanalysen durchgeführt und potentielle Entwicklungen über die Zeit aufgezeigt werden. Die VERA-Ergebnisse sind jedoch in den meisten Fällen nur auf der Bundeslandebene verfügbar. Dass es anders geht, zeigen die Bundesländer Berlin und Brandenburg, die in der Vergangenheit VERA-3-Ergebnisse unterhalb der Landesebene veröffentlicht haben (Berlin bis 2013/14 auf der Stadtbezirkseben und Brandenburg bis 2010/11 auf der Kreisebene). Die Transparenzbereitschaft wird wie folgt gewertet - die Maximalpunktzahl ist 3
        <ul>
            <li>auf Kreisebene / Bezirksebene veröffentlicht (3 Punktet)</li>
            <li>teilweise auf regionaler Ebene veröffentlicht (2 Punktet)</li>
            <li>nur auf Landesebene veröffentlicht (1 Punkt)</li>
        </ul>
      </p>

    </div>
  </div>
</template>

<script setup>
import categories from '@data/categories';

function getCategory(category) {
  return categories[category];
}
</script>