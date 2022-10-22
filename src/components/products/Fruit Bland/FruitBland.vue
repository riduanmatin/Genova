<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="p-8 lg:px-6 lg:py-12 xl:px-12">
      <h1 class="text-left text-black mb-2 font-semibold">Fruit Bland</h1>
      <hr class="h-1 rounded w-32 bg-black border-0" />
      <div
        class="grid grid-cols-1 md:grid-cols-3 justify-items-center justify-center gap-24 mt-10 mb-5"
      >
        <div class="" v-for="product in products" :key="product.id">
          <div class="flex flex-col h-fit background-yellow">
            <a href="#">
              <img
                :src="product.image.url"
                :alt="product.image.alt"
                class="h-60 w-56 object-contain rounded-t-xl"
              />
            </a>
            <div class="flex flex-col gap-3 p-5">
              <p
                class="text-base md:text-lg font-semibold text-black truncate block capitalize"
              >
                {{ product.name }}
              </p>
              <p class="text-base md:text-lg text-gray-600">
                RP. {{ product.price }}
              </p>
              <div class="">
                <button
                  class="rounded-lg px-4 py-1.5 bg-yellow-400 hover:bg-yellow-600 duration-300"
                >
                  Buy
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      products: [
        {
          id: 1,
          name: "Fruit Bland Manggo",
          image: {
            url: "  /assets/images/product/Syrup/syrup banana.png",
            alt: "I love you nature",
          },
          price: "97,000",
        },
        {
          id: 2,
          name: "Fruit Bland Manggo",
          image: {
            url: "../../../../assets/images/product/Syrup/syrup banana.png",
            alt: "I love you nature",
          },
          price: "97,000",
        },
        {
          id: 3,
          name: "Fruit Bland Manggo",
          image: {
            url: "../../../../assets/images/product/Syrup/syrup banana.png",
            alt: "I love you nature",
          },
          price: "97,000",
        },
      ],
    };
  },
};
</script>

<style scoped></style>
