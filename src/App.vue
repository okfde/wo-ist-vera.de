<template>
  <div>
    <div>
      <site-header />
      <transition name="fade" mode="out-in">
        <router-view class="mt-60 mb-16 flex-1" :key="$route.path" />
      </transition>
    </div>
    <site-footer />
  </div>
</template>

<script setup>
import { useHead } from '@vueuse/head';
import socialPreview from './assets/img/logo.png';
import favicon from './assets/img/favicon.png';

const title = 'Wo-ist-VERA.de - Transparenz für Vergleichsarbeiten';
const description =
  'Wo-ist-VERA.de vergleicht die Bundesländer im Umgang mit VERA-Daten.';

useHead({
  title,
  description,
  meta: [
    { property: 'og:image', content: socialPreview },
    { property: 'og:title', content: title },
    { property: 'og:description', content: description },
    { property: 'twitter:card', content: 'summary_large_image' }
  ],
  link: [
    {
      rel: 'icon',
      href: favicon
    }
  ]
});
</script>