<script setup lang="ts">
const config = useRuntimeConfig()
const appVersion = config.public.version

const yearCurrent = new Date().getFullYear()
</script>

<template>
  <footer class="p-4 flex flex-col md:flex-row justify-between items-center text-sm gap-4 md:gap-0">
    <div class="text-center md:text-left">
      © {{ yearCurrent }} Shane Carroll.
      Based on work by <NuxtLink aria-label="Website of Thorsten Seyschab" target="_blank" to="https://todde.tv/" class="underline">
      Thorsten Seyschab</NuxtLink>. (CC BY-SA 4.0).
      Modified version.
    </div>
    <div class="flex items-center space-x-4">
      <span>v{{ appVersion }}</span>
      <NuxtLink aria-label="Source Code on GitHub" target="_blank" to="https://github.com/skeryl/stage-flow-tools" class="flex items-center space-x-2 underline">
        <span>Source Code</span>
      </NuxtLink>
    </div>
  </footer>
</template>