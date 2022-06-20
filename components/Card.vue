<script setup>
const show = ref(false)
const show2 = ref(true)

if (window.innerWidth > 700) {
  show2.value = false
}
const minWidth = computed(() => {
  window.addEventListener('resize', () => {
    if (window.innerWidth > 700) {
      show2.value = false
    } else {
      show2.value = true
    }
  })
})
</script>

<style scoped>
.box {
  border: 1px solid limegreen;
}
</style>

<template>
  <v-card
    class="object-cover mx-auto   bg-black box mb-5 sm:cursor-pointer "
    max-width="344"
    min-width="344"
  >
    <v-img
      src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
      height="200px"
    ></v-img>

    <v-card-title>
      Top western road trips
    </v-card-title>

    <v-card-subtitle>
      1,000 miles of wonder
    </v-card-subtitle>

    <v-card-actions>
      <v-btn color="orange lighten-2" text>
        Explore
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn v-if="show2" icon @click="show = !show">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6 sm:hidden"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
          stroke-width="2"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19 9l-7 7-7-7"
          />
        </svg>
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <v-divider></v-divider>

        <v-card-text>
          I'm a thing. But, like most politicians, he promised more than he
          could deliver. You won't have time for sleeping, soldier, not with all
          the bed making you'll be doing. Then we'll go with that data file!
          Hey, you add a one and two zeros to that or we walk! You're going to
          do his laundry? I've got to find a way to escape.
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
</template>
