<!-- eslint-disable vue/require-v-for-key -->
<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="banner"></div>
    <div class="py-6 px-4 lg:px-6 lg:py-12 xl:px-12">
      <h1 class="text-left text-black mb-2 font-semibold">PRODUCTS</h1>
      <hr class="h-1 rounded w-28 bg-black border-0" />
      <div
        class="grid grid-cols-2 md:grid-cols-3 justify-items-center justify-center gap-y-6 mt-10 mb-5"
      >
        <div
          class="bg-yellow-200 flex flex-col h-fit bg-white shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Trending Flavors
            </p>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              New Flavors
            </p>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Beverage Boost
            </p>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Liquid Syrup
            </p>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Powder Syrup
            </p>
          </div>
        </div>

        <div
          class="flex flex-col bg-yellow-200 shadow-md rounded-xl duration-500 hover:scale-105 hover:shadow-xl"
        >
          <a href="#">
            <img
              src="../../assets/images/fruit bland mango.png"
              alt="Product"
              class="h-64 w-60 object-contain rounded-t-xl"
            />
          </a>
          <div class="p-5">
            <p class="text-lg font-bold text-black truncate block capitalize">
              Powder Drinks
            </p>
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
      cards: [1, 2, 3, 4, 5, 6, 7, 8],
      //   products: [
      //     {
      //       productTitle: "ABCN",
      //       image: [
      //         require("../../assets/images/fruit bland mango.png"),
      //         require("../../assets/images/fruit bland mango.png"),
      //       ],
      //       productId: 1,
      //     },
      //     {
      //       productTitle: "KARMA",
      //       image: [require("../../assets/images/fruit bland mango.png")],
      //       productId: 2,
      //     },
      //     {
      //       productTitle: "Tino",
      //       image: [require("../../assets/images/fruit bland mango.png")],
      //       productId: 3,
      //     },
      //     {
      //       productTitle: "EFG",
      //       image: [require("../../assets/images/fruit bland mango.png")],
      //       productId: 4,
      //     },
      //   ],
      innerStyles: {},
      step: "",
      transitioning: false,
    };
  },
  //   mounted() {
  //     this.setStep();
  //     this.resetTranslate();
  //   },

  //   methods: {
  //     setStep() {
  //       const innerWidth = this.$refs.inner.scrollWidth;
  //       const totalCards = this.cards.length;
  //       this.step = `${innerWidth / totalCards}px`;
  //     },

  //     next() {
  //       if (this.transitioning) return;

  //       this.transitioning = true;

  //       this.moveLeft();

  //       this.afterTransition(() => {
  //         const card = this.cards.shift();
  //         this.cards.push(card);
  //         this.resetTranslate();
  //         this.transitioning = false;
  //       });
  //     },

  //     prev() {
  //       if (this.transitioning) return;

  //       this.transitioning = true;

  //       this.moveRight();

  //       this.afterTransition(() => {
  //         const card = this.cards.pop();
  //         this.cards.unshift(card);
  //         this.resetTranslate();
  //         this.transitioning = false;
  //       });
  //     },

  //     moveLeft() {
  //       this.innerStyles = {
  //         transform: `translateX(-${this.step})
  //                     translateX(-${this.step})`,
  //       };
  //     },

  //     moveRight() {
  //       this.innerStyles = {
  //         transform: `translateX(${this.step})
  //                     translateX(-${this.step})`,
  //       };
  //     },

  //     afterTransition(callback) {
  //       const listener = () => {
  //         callback();
  //         this.$refs.inner.removeEventListener("transitionend", listener);
  //       };
  //       this.$refs.inner.addEventListener("transitionend", listener);
  //     },

  //     resetTranslate() {
  //       this.innerStyles = {
  //         transition: "none",
  //         transform: `translateX(-${this.step})`,
  //       };
  //     },
  //   },
};
</script>

<style scoped>
.carousel {
  width: 170px;
  overflow: hidden;
}

.inner {
  transition: transform 0.2s;
  white-space: nowrap;
}

/* optional */
button {
  margin-right: 5px;
  margin-top: 10px;
}
</style>
