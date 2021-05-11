<template>
  <div>
    <div class="w-11/12 md:w-4/5 m-auto mt-24 shadow">
      <div class="bg-black p-4">
        <h5 class="text-white font-bold text-xl text-center tracking-widest">
          OTHER THRILLING OFFERS
        </h5>
      </div>

      <div class="py-8 md:py-16 px-6 md:px-24 lists">
        <ul
          class="w-11/12 flex items-center py-4"
          v-for="item in items"
          :key="item.offers"
        >
          <svg
            class="svg-inline--fa fa-check fa-w-16 text-primary mr-2"
            width="24"
            height="24"
            aria-hidden="true"
            focusable="false"
            data-prefix="fa"
            data-icon="check"
            role="img"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 512 512"
            data-fa-i2svg=""
          >
            <path
              fill="#f16059"
              d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"
            ></path>
          </svg>

          <li
            class="flex list-none text-xs md:text-sm font-base text-gray-600 pl-3"
          >
            {{ item.offers }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          offers:
            '100% Money back guarantee if you didnt receive value worth your money.',
        },
        {
          offers:
            'Huge discount for first 20 participants! Course is worth 214$ but has been slashed to 55$ only.',
        },
        {
          offers:
            'Life time access to course, watch videos and read materials; anywhere, anytime.',
        },
        {
          offers:
            'You are indirectly helping the needy because a good percentage of sales will be given to charity or the poor.',
        },
        {
          offers:
            'At least 100% increment in profits guaranteed, as we have personally made over 700-800% profit. ',
        },
      ],
    }
  },
}
</script>

<style scoped>
.lists {
  display: grid;
}

@media (min-width: 768px) {
  .lists {
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>
