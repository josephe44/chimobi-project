<template>
  <div class="my-24 w-full md:w-10/12 m-auto">
    <h2
      class="m-auto font-bold text-center text-3xl w-11/12 md:w-4/5 md:text-4xl capitalize"
    >
      totally new to digital marketing? so were they!
    </h2>

    <div
      class="flex flex-col md:flex-row items-center bg-gray-100 py-10 lg:py-20 px-4 md:px-8 lg:px-16 w-10/12 md:w-full xl:px-20 mt-10 md:mt-12 m-auto shadow"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon icon-tabler icon-tabler-arrow-narrow-left"
        width="50"
        height="50"
        viewBox="0 0 24 24"
        stroke-width="1"
        stroke="#f16059"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <line x1="5" y1="12" x2="19" y2="12" />
        <line x1="5" y1="12" x2="9" y2="16" />
        <line x1="5" y1="12" x2="9" y2="8" />
      </svg>
      <ul
        class="flex flex-col lg:flex-row items-center lg:items-start w-5/6 max-w-5xl mt-12 mx-auto"
      >
        <li class="">
          <div class="w-32 lg:w-40 flex-shrink-0 pl-8">
            <div class="rounded-full overflow-hidden">
              <img
                width="701"
                height="669"
                src="https://s3.amazonaws.com/media.skillcrush.com/skillcrush/wp-content/uploads/2020/08/AMW_small-1-e1597780704411.png.webp"
                class="w-full h-full object-cover"
                alt=""
              />
            </div>
          </div>
          <blockquote class="mt-9 md:mt-0 md:mx-16 lg:mx-20">
            <h3
              class="font-bold font-display leading-tight uppercase text-center"
            >
              {{ displayTests[currentIndex].test_name }}
            </h3>
            <p class="mt-5 md:mt-8 lg:mt-2 lg:text-sm xl:text-base text-center">
              {{ displayTests[currentIndex].test_text }}
            </p>
            <p
              class="mt-6 md:mt-8 pt-6 border-t border-grey text-center lg:text-left"
            ></p>
          </blockquote>
        </li>
      </ul>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="icon icon-tabler icon-tabler-arrow-narrow-right"
        width="50"
        height="50"
        viewBox="0 0 24 24"
        stroke-width="1"
        stroke="#f16059"
        fill="none"
        stroke-linecap="round"
        stroke-linejoin="round"
        @click="currentIndex++"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <line x1="5" y1="12" x2="19" y2="12" />
        <line x1="15" y1="16" x2="19" y2="12" />
        <line x1="15" y1="8" x2="19" y2="12" />
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentIndex: 0,
      displayTests: [
        {
          test_name: 'Photosnap',
          test_text: 'Senior Frontend Developer',
        },
        {
          test_name: 'Manage',
          test_text: 'FullStack Developer',
        },
        {
          test_name: 'Account',
          test_text: 'Junior Frontend Developer',
        },
        {
          test_name: 'MyHome',
          test_text: 'Junior Frontend Developer',
        },
      ],
    }
  },
}
</script>
