<script setup>
import { ref } from "vue";
const projects = ref([
  {
    title: "Controle Financeiro",
    stacks: ["React"],
    resume: "Um CRUD para te ajudar no seu controle financeiro do dia a dia.",
    github: "https://github.com/shirator/Financas",
    demo: "https://react-entrega-s1-nu-kenzie-shirator.vercel.app/",
  },
  {
    title: "Title Project",
    stacks: ["React", "Tailwind", "Nest"],
    resume:
      "Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.",
  },
  {
    title: "Title Project",
    stacks: ["Vue", "SQL", "Golang"],
    resume:
      "Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.",
  },
]);
</script>

<template>
  <div
    class="font-semibold text-2xl text-center uppercase pb-4 text-white"
    ref="projectRef"
  >
    Projetos
  </div>
  <div class="flex justify-center">
    s
    <div class="w-2/3 flex flex-col gap-10">
      <div
        v-for="(project, index) in projects"
        key="index"
        class="bg-gray-100 p-6 rounded-sm flex gap-3 flex-col shadow-2xl shadow-purple-600"
      >
        <p class="uppercase text-lg font-semibold">{{ project.title }}</p>
        <div class="flex gap-3">
          <span
            v-for="stack in project.stacks"
            class="bg-purple-600 text-xs uppercase py-2 px-1 text-white font-semibold rounded-sm"
          >
            {{ stack }}
          </span>
        </div>
        <p class="text-justify">{{ project.resume }}</p>
        <div class="flex flex-col gap-2">
          <button
            class="py-3 px-5 bg-gradient-to-r from-purple-700 to-pink-500 rounded-md text-white uppercase font-medium"
          >
            <a :href="project.github" target="_blank">Code</a>
          </button>
          <button
            class="py-3 px-5 bg-gradient-to-r from-purple-700 to-pink-500 rounded-md text-white uppercase font-medium"
          >
            <a :href="project.demo" target="_blank">Demo</a>
          </button>
        </div>
      </div>
    </div>
  </div>

  <div class="pt-10 flex justify-center">
    <button
      class="py-3 px-5 bg-gradient-to-r from-purple-700 to-pink-500 rounded-md text-white uppercase font-medium"
    >
      Veja todos os meus projetos
    </button>
  </div>
</template>
