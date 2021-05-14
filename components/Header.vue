<template>
  <div class="bg-gray-300 w-screen sticky top-0 opacity-99">
    <div class="py-4 px-8 flex flex-wrap justify-between items-center">
      <div class="flex items-center">
        <!-- <img src="" width="50" alt="Logo" class="" /> -->
        <div class="w-20 h-10 bg-gray-400"></div>
      </div>
      <button
        class="block md:hidden menu-toggle"
        @click="showDropDown = !showDropDown"
      >
        <svg
          v-if="!showDropDown"
          xmlns="http://www.w3.org/2000/svg"
          class="icon icon-tabler icon-tabler-menu-2"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="#f16059"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
          <line x1="4" y1="6" x2="20" y2="6" />
          <line x1="4" y1="12" x2="20" y2="12" />
          <line x1="4" y1="18" x2="20" y2="18" />
        </svg>
        <svg
          v-else
          xmlns="http://www.w3.org/2000/svg"
          class="icon icon-tabler icon-tabler-x"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="#2c3e50"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
          <line x1="18" y1="6" x2="6" y2="18" />
          <line x1="6" y1="6" x2="18" y2="18" />
        </svg>
      </button>

      <div class="font-medium hidden md:flex md:justify-between">
        <a
          v-for="(link, index) in headerLinks"
          :key="index"
          :href="link.link"
          class="py-2 px-4 text-gray-600 block md:inline-block"
          >{{ link.name }}</a
        >
      </div>
    </div>
    <div
      v-if="showDropDown"
      class="font-medium block lg:hidden border-t-2 border-gray-200"
    >
      <a
        v-for="(link, index) in headerLinks"
        :key="index"
        :href="link.link"
        class="py-2 px-4 text-gray-600 block text-center md:inline-block"
        >{{ link.name }}</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      showDropDown: false,
      headerLinks: [
        {
          link: '/',
          name: 'Home',
        },
        {
          link: '#about',
          name: 'About us',
        },
        {
          link: '#services',
          name: 'Services',
        },
        {
          link: '#testimonials',
          name: 'Testimonials',
        },
        {
          link: '#payment',
          name: 'Payment',
        },
      ],
    }
  },
}
</script>

<style scoped>
*:focus {
  outline: none !important;
}
</style>
