
<script setup lang="ts">
import Index from '../components/home.vue';

const links = [{
  label: 'About',
  to: 'https://ui.nuxt.com/'
}, {
  label: 'Comming soon',
  to: 'https://nuxt.com'
}, {
  label: 'Contribute',
  to: 'https://nuxt.studio'
}]

const nav = [
  { label: 'home', to: '/' },
  { label: 'Forbidden', to: '/forbidden' },
  { label: 'Redirect', to: '/redirect' },
]


// const route = useRoute()
</script>
<template>
  
  <body class="bg-slate-950" :nav="nav">
    <head>
      <title>Cube Miner </title>
      <Meta name="description" content="Official | Cube Miner Team" />
      <Meta name="keywords" content="Bitcoin, Crypto, Money, Minning, Mining"</Meta>
      <Meta name="robots" content="index, follow"/>

    </head>
    <Index />

  </body>
  
    
    
</template>./components/home.vue