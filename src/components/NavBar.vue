<script setup>
function scrollToProjects() {
  this.$refs.projectRef.scrollIntoView({ behavior: "smooth" });
  console.log(this.$refs);
}
</script>

<template setup>
  <div
    class="text-white flex justify-between bg-black-primary p-4 items-center font-medium lg:px-20"
  >
    <div class="font-semibold uppercase text-lg">Carlos Mesquita &lt / ></div>
    <div class="flex gap-4 items-center">
      <button @click="scrollToProjects">Projetos</button>
      <div>
        <button
          class="py-3 px-5 bg-gradient-to-r from-purple-700 to-pink-500 rounded-md"
        >
          <a
            href="https://drive.google.com/file/d/1xeWGkKnS5XjUn5k1x8zZZu1UMHqcEC1G/view?usp=sharing"
            target="_blank"
            >Download CV</a
          >
        </button>
      </div>
    </div>
  </div>
</template>
