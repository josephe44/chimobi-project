<template>
  <div>
    <div class="bg-white py-4 px-8 mt-8 flex justify-around items-center">
      <div class="">
        <img
          src="https://res.cloudinary.com/audrepx100/image/upload/v1619774310/box-images_iktahw.png"
          width="100%"
          alt="Featured"
          class=""
        />
      </div>

      <div class="text-gray-700 w-2/5 pl-12">
        <h3 class="pb-4 font-extrabold text-4xl">
          We care about our customers
        </h3>
        <p class="text-base font-medium w-11/12 leading-7">
          Compilation of a world class Google ads course that teaches you the
          indepth secrets and operational systems of advertising and getting
          results from a beginner level to an advanced level.The training comes
          in 3 phases: 6 courses, Advanced Google ads and lifetime mentorship.
          Participants will get training on Google analytics, Google ads, and
          Youtube all for free!
        </p>
      </div>
    </div>

    <div class="w-4/5 bg-gray-50 m-auto pt-14 pl-14 mt-8 rounded-2xl">
      <ul
        class="w-11/12 flex justify-start items-center pb-8"
        v-for="item in items"
        :key="item.offers"
      >
        <img
          class="checkbox"
          src="https://res.cloudinary.com/softnexus/image/upload/v1596465127/assets/images/icons/Checkbox_p1dkio.svg"
          alt="☑"
        />

        <li class="flex list-none text-xl font-bold text-gray-600 pl-8">
          {{ item.offers }}
        </li>
      </ul>
    </div>

    <div class="w-4/6 m-auto text-gray-700 w-full mt-20">
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
.checkbox img {
  max-width: 5%;
}
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
</style>
