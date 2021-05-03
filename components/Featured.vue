<template>
  <div>
    <div
      class="bg-white py-4 px-8 mt-8 md:flex md:justify-around items-center flex-col"
    >
      <div class="">
        <img
          src="https://res.cloudinary.com/audrepx100/image/upload/v1619774310/box-images_iktahw.png"
          width="100%"
          alt="Featured"
          class=""
        />
      </div>

      <div class="text-gray-700 w-11/12 md:w-2/5 md:pl-12">
        <h3 class="md:pb-4 font-extrabold text-4xl text-center">
          We care about our customers
        </h3>
        <p class="text-base font-medium md:w-11/12 leading-7 text-center">
          Compilation of a world class Google ads course that teaches you the
          indepth secrets and operational systems of advertising and getting
          results from a beginner level to an advanced level.The training comes
          in 3 phases: 6 courses, Advanced Google ads and lifetime mentorship.
          Participants will get training on Google analytics, Google ads, and
          Youtube all for free!
        </p>
      </div>
    </div>

    <!-- <div class="w-4/5 bg-gray-50 m-auto pt-14 pl-14 mt-8 rounded-2xl">
      <ul
        class="w-11/12 flex justify-start items-center pb-8"
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

        <li class="flex list-none text-xl font-bold text-gray-600 pl-8">
          {{ item.offers }}
        </li>
      </ul>
    </div> -->

    <div class="w-4/5 m-auto mt-16 relative">
      <div class="bg-black p-4">
        <h5 class="text-white font-bold text-xl text-center tracking-widest">
          OTHER THRILLING OFFERS
        </h5>
      </div>

      <div class="py-16 px-24 lists">
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

          <li class="flex list-none text-xs font-base text-gray-600 pl-3">
            {{ item.offers }}
          </li>
        </ul>
      </div>
    </div>

    <div class="absolute w-4/6 m-auto bg-gray-50 text-gray-700 w-full -m-16">
      <h3 class="w-1/3 pb-4 m-auto font-extrabold text-4xl text-center">
        Ready to begin your success story?
      </h3>
      <p class="w-3/4 text-center text-base font-medium m-auto leading-7">
        Looking to learn advanced Google ads focusing on Optimisation, ranking
        ads, getting conversions, getting clients, minimizing ad spend,
        targeting audiences, Google ads Optimisation tools, Advanced Google ads?
        Want to learn both? it costs 110$ only.
      </p>
      <button
        class="text-white font-bold flex items-center text-center rounded-3xl py-3 px-8 mt-8 m-auto cursor-pointer bounce"
      >
        <a href="">Learn Advanced Google Ads Now</a>
      </button>
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
button {
  background: linear-gradient(
    141.27deg,
    #f5b72f 4.56%,
    #bd2467 57.6%,
    #2497c3 90.86%
  );
  box-shadow: inset 3.44px 5.44px 19.3906px 6.84375px rgba(255, 255, 255, 0.79);
}

.bounce:hover {
  animation: bounce 1s;
  -webkit-animation: bounce 1s;
}

@keyframes bounce {
  0% {
    border-radius: 15px;
  }
  20% {
    border-radius: 30px;
  }
  60% {
    border-radius: 20px;
    transform: scale(1.1);
    -ms-transform: scale(1.1); /* IE 9 */
    -webkit-transform: scale(1.1); /* Safari and Chrome */
  }
  90% {
    transform: scale(0.98);
    -ms-transform: scale(0.98); /* IE 9 */
    -webkit-transform: scale(0.98); /* Safari and Chrome */
  }
  100% {
    border-radius: 15px;
  }
}

@-webkit-keyframes bounce {
  0% {
    border-radius: 15px;
  }
  20% {
    border-radius: 30px;
  }
  60% {
    border-radius: 20px;
    transform: scale(1.1);
    -ms-transform: scale(1.1); /* IE 9 */
    -webkit-transform: scale(1.1); /* Safari and Chrome */
  }
  90% {
    transform: scale(0.98);
    -ms-transform: scale(0.98); /* IE 9 */
    -webkit-transform: scale(0.98); /* Safari and Chrome */
  }
  100% {
    border-radius: 15px;
  }
}

.lists {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}

.lists:nth-child(odd) {
  border-color: black;
  border-right: 1px black;
  border-style: solid;
}
</style>
