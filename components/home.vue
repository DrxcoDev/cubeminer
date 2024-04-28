<script setup lang="ts">

const links = [{
  label: 'About',
  to: '/about'
}, {
  label: 'Comming soon',
  to: '/commingsoon'
}, {
  label: 'Contribute',
  to: 'https://nuxt.studio'
}]
</script>
<template>
    <ULandingHero
    title="Cube Miner"
    description="Get everything that is yours quickly and without risks in an anonymous way. Mine without stopping. Our crypto website 3.0 will make you happy"
    orientation="horizontal"
    :links="[{ label: 'Read More', icon: 'i-heroicons-cube', color: 'indigo', size: 'lg', to: '../about' }]"
  >
    <template #headline>
      <NuxtLink to="/commingsoon">
        <UButton
        color="indigo"
        to=""
        label="Cooming soon!"
        trailing-icon="i-heroicons-arrow-right"
        size="xl"
        class="rounded-full transition ease-in-out bg-indigo-900 hover:translate-x-20 hover:scale-110 hover:bg-indigo-500 duration-300"
      />
      </NuxtLink>
      
    </template>
    <template #default>
      <img
        src="https://static.vecteezy.com/system/resources/previews/011/993/940/original/cube-3d-shape-gradient-illustration-in-trendy-color-the-colorful-shapes-creative-element-in-contemporary-style-png.png"
        class="w-full rounded-mddark:ring-gray-700"
      
      />
    </template>
    
  </ULandingHero>

  <!-- Section main  -->
  <ULandingSection
  title="The blockchain"
  description="Have fun mining our virtual currency. The first Spanish in the world?"
  align="right"
>
  <img
    src="https://img.freepik.com/foto-gratis/mano-masculina-ethereum-dorado-sobre-fondo-azul_155003-8466.jpg?w=740&t=st=1714162169~exp=1714162769~hmac=b92969d7a3736f52ae41ba7fe4e4f954cdfb057733ac4804b584b19653acfb68"
    class="w-full rounded-md "
  />
</ULandingSection>
<ULandingSection
  title="Our Servers"
  description="Servers that give responses in seconds. We have support 24 hours a day"
  align="left"
  >
  <img
    src="https://img.freepik.com/vector-gratis/concepto-procesamiento-datos-grandes-sala-servidores-acceso-token-tecnologia-blockchain_39422-812.jpg?t=st=1714163056~exp=1714166656~hmac=3cee0eeadab401a00c2744a0f9ccee6c59d69003b8ee69f3275dc5c115a7004c&w=740"
    class="w-full rounded-md "
  />
</ULandingSection>

  <!-- footer -->
  <UFooter :links="links">
    <template #left>
      Copyright © {{ new Date().getFullYear() }} | Nexus Team
    </template>

    <template #right>
      <UButton icon="i-simple-icons-x" color="gray" variant="ghost" to="https://x.com/nuxt_js" target="_blank" />
      <UButton icon="i-simple-icons-discord" color="gray" variant="ghost" to="https://discord.com/invite/ps2h6QT" target="_blank" />
      <UButton icon="i-simple-icons-github" color="gray" variant="ghost" to="https://github.com/nuxt/nuxt" target="_blank" />
    </template>
  </UFooter>


    
    
</template>