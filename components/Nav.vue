<template>
  <nav
    class="h-[9vh] mb-5  bg-black box 
    text-center
    flex
    items-center
    justify-center
    "
  >
    <ul class="text-white">
      <li>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6 inline-block mb-1 text-purple-600"
          viewBox="0 0 20 20"
          fill="currentColor"
        >
          <path
            fill-rule="evenodd"
            d="M12.395 2.553a1 1 0 00-1.45-.385c-.345.23-.614.558-.822.88-.214.33-.403.713-.57 1.116-.334.804-.614 1.768-.84 2.734a31.365 31.365 0 00-.613 3.58 2.64 2.64 0 01-.945-1.067c-.328-.68-.398-1.534-.398-2.654A1 1 0 005.05 6.05 6.981 6.981 0 003 11a7 7 0 1011.95-4.95c-.592-.591-.98-.985-1.348-1.467-.363-.476-.724-1.063-1.207-2.03zM12.12 15.12A3 3 0 017 13s.879.5 2.5.5c0-1 .5-4 1.25-4.5.5 1 .786 1.293 1.371 1.879A2.99 2.99 0 0113 13a2.99 2.99 0 01-.879 2.121z"
            clip-rule="evenodd"
          />
        </svg>
      </li>
      <li class="md:pl-3 lg:pl-6 xl:pl-16"><a href="#">HeatCode</a></li>
      <li class="md:pl-3 lg:pl-6 xl:pl-16"><a href="#">About</a></li>
      <li class="md:pl-3 lg:pl-6 xl:pl-16 cursor-pointer">
        <NuxtLink to="/card">card</NuxtLink>
      </li>
      <li class="md:pl-3 lg:pl-6 xl:pl-16"><a href="#">Contact</a></li>
      <li class="md:pl-5 lg:pl-6 xl:pl-16">
        <div
          class="inline-block border-b-fuchsia-700/50 border-l-green-700/50 border-t-pink-500/50 border-cyan-500/50 hover:border-b-fuchsia-500 hover:border-l-green-700 hover:border-t-pink-500 hover:border-cyan-500 border-2 pb-1 px-2  rounded-md cursor-pointer hover:scale-110 transition-all duration-200 active:scale-95"
        >
          <a href="#">login</a>
        </div>
      </li>
    </ul>
  </nav>
</template>

<script setup>
const router = useRouter()
const nCard = () => {
  router.push({ path: '/card' })
}
</script>

<style scoped>
li {
  display: inline;
  padding-left: 10px;
}

.box {
  border-bottom: 1px solid limegreen;
}
</style>
