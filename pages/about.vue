<script setup lang="ts">

const links = [{
  label: 'Home',
  to: '/app'
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
      title="About"
      description=""
    />
    <ULandingSection
      headline=""
      title="About our company"
      description="Who are we?From where?Well, we are a team that is passionate about the blockchain tecnology and Web3.0. We in this year have created a new mining plataform of cryptocurrency.Now we are finished with the development of the plataform and we are going to launch it in the next times..."
      align="left"
    >
      <!-- <img
        src="https://picsum.photos/640/360"
        class="w-full rounded-md shadow-xl ring-1 ring-gray-300 dark:ring-gray-700"
      /> -->
    </ULandingSection>
    <ULandingSection
      headline=""
      title="New cryptocurrency"
      description="This project is centralized in the creation of our new cryptocurrency called Blockly.Actually don't working, because we are working in the development of the platform yet."
      align="right"
    >
      <!-- <img
        src="https://picsum.photos/640/360"
        class="w-full rounded-md shadow-xl ring-1 ring-gray-300 dark:ring-gray-700"
      /> -->
      <div class="" style="padding:20px">
        <UCard style="padding: 10px;width:300px;">
            <template #header>
                <div class="flex justify-between">
                    <div>
                        <h3 class="text-xl font-semibold text-teal-300">Blockly Tecnology</h3>
                    </div>
                    
                </div>
            </template>
            <Placeholder class="h-8" />
            
            <p>Our cryptocurrency, Blockly, has created with the news tecnologies.</p>
        
            <Placeholder class="h-32" />
        
            <template #footer>
            <div class="flex justify-between mt-2">
                <span class="rounded-md border px-3 text-emerald-500 border-emerald-500 mx-4">#Nuxt</span> <br>
                <span class="rounded-md border px-3 text-sky-700 border-sky-700 mx-4">#TypeScript</span>

            </div>
            <div class="flex justify-between mt-2">
                <span class="rounded-md border px-3 text-green-400 border-green-400 mx-4">#Vue</span>
                <span class="rounded-md border px-3 text-amber-500 border-amber-500 mx-4">#Rust</span>
            </div>
            <div class="flex justify-between mt-2">

                <span class="rounded-md border px-3 text-sky-300 border-sky-300 mx-4">#Go</span>
            </div>
            <Placeholder class="h-8" />
            </template>
        </UCard>
    </div>
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
  