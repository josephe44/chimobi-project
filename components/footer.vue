<template>
  <div id="payment" class="bg-gray-50">
    <div class="w-4/6 m-auto mt-96 pt-12 text-gray-700 w-full">
      <h3
        class="md:w-1/3 pb-4 m-auto font-extrabold text-3xl md:text-4xl text-center"
      >
        Ready to begin your success story?
      </h3>
      <p
        class="w-11/12 md:w-3/4 text-center text-base font-medium m-auto leading-7"
      >
        Looking to learn advanced Google ads focusing on Optimisation, ranking
        ads, getting conversions, getting clients, minimizing ad spend,
        targeting audiences, Google ads Optimisation tools, Advanced Google ads?
        Want to learn both? it costs 110$ only.
      </p>
      <button
        class="text-white font-bold flex items-center text-center rounded-3xl py-3 px-16 mt-8 m-auto cursor-pointer bounce"
      >
        <a href="">Get Course Now</a>
      </button>
    </div>

    <div class="pt-60 pb-4 items-center">
      <p class="text-center text-gray-700 font-bold">
        © 2020 Chimaobi Ifenkwe Enterprises
      </p>
      <!-- <div class="pr-24 flex">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="icon icon-tabler icon-tabler-mail"
          width="28"
          height="28"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="#ffffff"
          fill="#9CA3AF"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
          <rect x="3" y="5" width="18" height="14" rx="2" />
          <polyline points="3 7 12 13 21 7" />
        </svg>
        <a class="pl-2 text-gray-50" href="mailto:loverofart10@yahoo.com"
          >send a mail</a
        >
      </div> -->
    </div>
    <div
      style="z-index: 214748364 !important; left: auto; right: 15px"
      class="floating-wpp"
      @click="goToWhatsapp()"
    >
      <div
        class="floating-wpp-button"
        style="width: 60px; height: 60px; background-color: rgb(37, 211, 102)"
      >
        <img
          src="https://rawcdn.githack.com/rafaelbotazini/floating-whatsapp/3d18b26d5c7d430a1ab0b664f8ca6b69014aed68/whatsapp.svg"
        />
        <div class="floating-wpp-button-image"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    goToWhatsapp() {
      this.$router.push('/https://wa.me/2348166757438')
    },
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

.floating-wpp {
  position: fixed;
  bottom: 15px;
  left: 15px;
  font-size: 14px;
  transition: bottom 0.2s;
}

.floating-wpp:hover {
  bottom: 17px;
}

.floating-wpp:hover .floating-wpp-button {
  box-shadow: 1px 2px 8px rgb(60 60 60 / 40%);
}

.floating-wpp .floating-wpp-button {
  position: relative;
  border-radius: 50%;
  box-shadow: 1px 1px 4px rgb(60 60 60 / 40%);
  transition: box-shadow 0.2s;
  cursor: pointer;
  overflow: hidden;
  background-color: rgb(37, 211, 102);
}

.floating-wpp .floating-wpp-button img,
.floating-wpp .floating-wpp-button svg {
  position: absolute;
  width: 100%;
  height: auto;
  object-fit: cover;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -50%, 0);
}

img {
  outline: none;
}
</style>
