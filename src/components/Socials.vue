<script setup lang="ts">
import Github from "../components/icons/Github.vue";
import Gmail from "../components/icons/Gmail.vue";
import Linkedin from "../components/icons/Linkedin.vue";
</script>

<template>
  <div class="text-white pt-14 uppercase px-12">
    <p class="font-semibold text-2xl text-center pb-4">Redes Sociais</p>
    <div class="flex justify-center pt-7 pb-20 gap-5">
      <div class="flex flex-col items-center gap-2"><Gmail />Gmail</div>
      <div class="flex flex-col items-center gap-2"><Linkedin />Linkedin</div>
      <div class="flex flex-col items-center gap-2"><Github />Github</div>
    </div>
  </div>
</template>
