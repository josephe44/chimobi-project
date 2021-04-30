<template>
  <div>
    <div class="bg-white py-4 px-8 flex justify-around items-center">
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
    <div
      class="w-4/5 h-60 bg-gray-50 m-auto py-4 px-4 mt-8 rounded-2xl flex items-center"
    >
      <div class="">
        <img
          class="checkbox"
          src="https://res.cloudinary.com/softnexus/image/upload/v1596465127/assets/images/icons/Checkbox_p1dkio.svg"
          alt="☑"
        />
        <span> {{ text.description }} </span>
      </div>
    </div>
  </div>
</template>
