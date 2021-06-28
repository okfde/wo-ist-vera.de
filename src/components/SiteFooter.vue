<template>
  <footer class="bg-darkblue text-light">
    <div class="max-w-screen-xl mx-auto px-4 py-8">
      <h2 class="text-3xl mb-8 mt-2 md:mt-8 font-semibold">
        Über <i>Wo ist VERA?</i>
      </h2>

      <div class="w-full prose prose-md prose-dark">
        <div class="footer-grid">
          <div>
            <h3>Die Erhebung</h3>
            <p>
              Nur wenige Bundesländer veröffentlichen VERA-Daten. In der Regel werden sie lediglich den Schulen zurückgespiegelt. Dabei sind sie wichtige Instrumente für die Bewertung, Erforschung und Entwicklung von Schulbildung. Wir bündel die Daten und machen den Umgang der Bundesländer mit diesen sichtbar.
            </p>

          </div>

          <div>
            <h3>Das Projekt</h3>
            <p>
              Wo-ist-VERA.de ist ein Projekt des Open Knowledge Foundation Deutschland e. V. Der Quellcode ist zu finden
              <a target="_blank" href="https://github.com/okfde/wo-ist-vera.de"
                >auf Github</a
              >. Verwendete Tools sind Vue.js und Tailwind CSS.
            </p>
            <div class="flex items-center">
              <a href="https://okfn.de" target="_blank" class="w-1/2">
                <img
                  class="mr-6 h-auto object-contain max-h-24"
                  src="../assets/img/okfde.svg"
                  alt="Open Knowledge Foundation Deutschland e.V."
                />
              </a>
            
            </div>
          </div>
        </div>

        <div class="footer-grid">
          <div>
            <h3>Downloads</h3>
            <div class="footer-grid">
              <p>
                <i-mdi-github class="mr-1" />
                <a target="_blank" href="https://github.com/okfde/wo-ist-vera.de"
                  >Quellcode & Datensatz
                </a>
              </p>
            </div>
          </div>
          <div>
            <h3>Copyright</h3>
            <p>
              Dieses Werk und die Daten sind lizenziert unter Creative Commons
              Namensnennung 4.0 International (<a
                href="https://creativecommons.org/licenses/by/4.0/"
                >CC BY 4.0</a
              >).
            </p>
          </div>
        </div>

        <div class="footer-grid">
          <div>
            <h3>Kontakt</h3>
            <p>
              Wir freuen uns sehr über Feedback, Kritik und Fragen. Kontaktieren
              Sie uns bitte unter
              <a href="mailto:info@okfn.de">dieser Mail-Adresse</a>
            </p>
          </div>
          <div>
            <h3>Impressum</h3>
            <p>
              Verantwortlicher Diensteanbieter für diese Homepage ist der
              Open Knowledge Foundation Deutschland e. V.
            </p>
            <p>
              <a target="_blank" href="https://okfn.de/impressum/">Impressum</a>

              <a target="_blank" href="https://okfn.de/impressum/#datenschutzerkl%C3%A4rung">
                Datenschutzerklärung
              </a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
</script>

<style lang="postcss" scoped>
footer .footer-grid {
  @apply md:grid grid-cols-2 gap-x-4;
}
</style>