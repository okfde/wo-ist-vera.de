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
        In Deutschland wird Bildungspolitik in einer Blackbox gemacht. Es gibt kaum Länder, die so wenig über ihr Schulsystem wissen, wie Deutschland. Und die wenigen Daten, die vorliegen, halten die Bundesländer weitestgehend unter Verschluss. Wie problematisch das ist, zeigt sich gerade besonders: Alle reden über pandemiebedingte Lernrückstände, aber inwiefern die genau existieren, weiß niemand so genau - weil die Daten nicht vorliegen. Wie sollen so effektive Maßnahmen ergriffen werden?
        </p>
        <p>
        Dabei werden Daten erhoben und das schon seit Jahren. Die sogenannten VERgleichsArbeiten (kurz VERA) sind weitestgehend standardisierte Kompetenztests. Mit ihnen werden Grundkompetenzen erhoben, wie Lesefähigkeit, Schreibfähigkeit oder mathematische Grundkenntnisse. Auf Wo-ist-VERA.de veröffentlichen wir zum ersten Mal vorhandene Daten an einem zentralen Ort und wollen eine Diskussion über ihre Nutzbarkeit initiieren. Außerdem machen wir über ein Ranking sichtbar, welche Bundesländer bei der Veröffentlichung blockieren.
        </p>
        <p>
        Sie können <router-link to="/methodik/">hier</router-link> mehr über
        unsere Kriterien zur Erfassung des Rankings erfahren.
        </p>
        <ranking-map />
        <p><i>„Anonymisierte schulische Leistungsdaten sollten grundsätzlich allen.. Menschen zur Verfügung gestellt werden. Schule ist eine öffentliche.. Veranstaltung - also sollten auch alle.. so fundiert und differenziert wie möglich Einblick erhalten.“</i><br><strong>Jens Großpietsch</strong>, ehem. Schulleiter Heinrich von Stephan Gemeinschaftsschule, Mitbegründer der Freudberg Gemeinschaftsschule in Berlin.</p>

        <p><i>„Wir müssen als Gesellschaft entscheiden, welche Erwartungen wir.. an Schulen haben.. Wenn wir uns an einem Ziel orientieren, dann sind Lernstandserhebungen ein geeignetes Mittel, den Weg zum Ziel zu überprüfen.. Für eine Veröffentlichung der VERA-Daten spricht, dass es sowohl den Eltern als auch anderen Bildungsinteressierten möglich sein sollte, die Erreichung der Ziele zu überprüfen.“</i><br><strong>Katja Oltmanns</strong>, Vorsitzende der Landeselternvertretung der Gymnasien im Saarland, Deligierte des Bundeselternrates.</p>

    </div>
  </div>
</template>
