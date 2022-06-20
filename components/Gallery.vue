<template>
  <div class="grid px-2 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3 ">
    <div
      v-for="n in 9"
      class="p-2 box m-2 rounded group hover:scale-105  transition-all duration-100 ease-in"
    >
      <img
        class="mb-2 w-full object-cover "
        :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
        alt=""
      />
      <div>
        <h3 class="text-emerald-700 group-hover:text-emerald-400">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
        </h3>
      </div>
    </div>
  </div>
</template>
<script setup></script>

<style scoped>
.box {
  border-color: green;
  border: 1px solid green;
}
</style>
