<template>
  <div class="container state" v-if="state">
    <h1 class="headline">{{ state.name }}</h1>
    <div class="prose">
      <div class="text-center italic">
              <p v-if="state.datalink">
                Mit der Wertung nicht zufrieden? Stellen Sie eine <a href="https://fragdenstaat.de/info/informationsfreiheit/einfuehrung/" target="_blank">Informationsfreiheits-Anfrage</a> und sorgen Sie für mehr Transparenz!
                <a
                  :href="`https://fragdenstaat.de/behoerde/${state.fds.slug}/`"
                  class="link whitespace-nowrap"
                >
                Anfrage stellen
                </a>
              </p>
              <p v-else>{{state.name}} hält VERA-Daten bisher unter Verschluss.</p>
            </div>
    </div>

    <table class="ranking-bars">
      <tr
        v-for="(bar, i) in performance"
        :key="bar.category.slug"
        :class="{ first: i === 0 }"
      >
        <td>
          <span :class="{ 'font-bold': i === 0 }">
            <router-link
              :to="`#${bar.category.slug}`"
              v-if="i !== 0"
              title="Mehr Informationen..."
            >
              {{ bar.category.title }}

              <i-mdi-information-outline />
            </router-link>
            <span v-else v-text="bar.category.title" />
          </span>
        </td>
        <td class="w-full">
          <ranking-bar :color="bar.category.color" :progress="bar.percentage" />
        </td>
      </tr>
    </table>


    <state-details v-if="state.criteria" :performance="performance" />

    <div class="text-center italic" v-if="state.info">
        <br><strong>Weitere Informationen</strong>
        <p>{{ state.info }}</p>
    </div>
    <div class="btn-wrap" v-if="state.datalink">
       <a target="_blank" class="btn black" :href="`${state.datalink}`">VERA-Daten Herunterladen</a>
    </div>
    <div class="btn-wrap" v-else>
        <p>{{state.name}} hält VERA-Daten bisher unter Verschluss. Stellen Sie eine Anfrage nach dem <a href="https://fragdenstaat.de/info/informationsfreiheit/einfuehrung/" target="_blank">Informationsfreiheitsgesetz</a> und engagieren Sie sich für mehr Transparenz!</p><br>
        <a :href="`https://fragdenstaat.de/behoerde/${state.fds.slug}/`" target="_blank" class="btn black">Anfrage stellen</a>
    </div>
  </div>
</template>

<script setup>
import { computed, defineProps } from 'vue';
import { useHead } from '@vueuse/head';

import lawtypes from '~/data/lawtypes.yml';
import states from '@data/states';
import _categories from '@data/categories';

const categories = Object.values(_categories);

const props = defineProps({
  state: {
    type: String,
    required: true
  }
});

function getCategory(categorySlug = 'gesamt') {
  return categories.find(c => c.slug === categorySlug);
}

const state = computed(() => states.find(s => s.slug === props.state));
const law = computed(() => lawtypes[state.value.type]);

const performance = computed(() =>
  state.value.performance.map(p => ({
    ...p,
    category: getCategory(p.categorySlug)
  }))
);

const stateName =
  state.value.name === 'Bund' ? 'Deutschland' : state.value.name;
const title = `Informationsfreiheit in ${stateName} - Das Transparenzranking`;
useHead({ title });
</script>

<style scoped>
.state:deep() h2 {
  @apply text-xl md:text-3xl font-semibold mt-6 mb-1;
}
</style>