<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="banner"></div>
    <div class="py-6 px-4 lg:px-6 lg:py-12 xl:px-12">
      <h1 class="text-left text-black mb-2 font-semibold">PRODUCTS</h1>
      <hr class="h-1 rounded w-28 bg-black border-0" />
      <div
        class="grid grid-cols-2 md:grid-cols-3 justify-items-center justify-center gap-6 mt-10 mb-5"
      >
        <div
          class="bg-yellow-200 flex flex-col h-fit bg-white shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit_bland_kiwi.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Trending Flavors
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit_bland_passion fruit.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              New Flavors
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit_bland_raspberry.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Beverage Boost
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit_bland_strawberry.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Liquid Syrup
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/syrup_vanilla-removebg-preview.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Powder Syrup
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/syrup_strawberry-removebg-preview.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Powder Drinks
            </p>
            <div class="mt-6">
              <button
                class="rounded-lg px-4 py-2 bg-yellow-400 hover:bg-yellow-600 duration-300"
              >
                See More
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  components: {},
  data() {
    return {};
  },
};
</script>
<style scoped></style>
