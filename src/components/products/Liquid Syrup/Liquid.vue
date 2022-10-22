<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <section class="container mx-auto">
    <div class="p-8 lg:px-6 lg:py-12 xl:px-12">
      <h1 class="text-lg text-left text-black mb-2 font-semibold md:text-xl">
        Liquid Syrup
      </h1>
      <hr class="h-1 rounded w-32 bg-black border-0" />
      <div
        class="grid grid-cols-1 md:grid-cols-3 justify-items-center justify-center gap-24 mt-10 mb-5"
      >
        <div class="" v-for="product in products" :key="product.id">
          <div
            class="flex flex-col h-fit background-yellow md:-p-2 md:rounded-xl"
          >
            <a href="#">
              <img
                :src="product.image"
                :alt="product.name"
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
          name: "Syrup Pineapple",
          image: "syrup pineapple.png",
          price: "97,000",
        },
        {
          id: 2,
          name: "Syrup Raspberry",
          image: "syrup raspberry.png",
          price: "97,000",
        },
        {
          id: 4,
          name: "Syrup Banana",
          image: "syrup_banana-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 5,
          name: "Syrup Blue Curacao",
          image: "syrup_blue_curacao-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 6,
          name: "Syrup Bubblegum",
          image: "syrup_bubble_gum-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 7,
          name: "Syrup Butterscotch",
          image: "syrup_butterscotch-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 8,
          name: "Syrup Caramel",
          image: "syrup_caramel-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 9,
          name: "Syrup Coconut",
          image: "syrup_coconut-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 10,
          name: "Syrup Ginger",
          image: "syrup_ginger-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 11,
          name: "Syrup Green Apple",
          image: "syrup_green_apple-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 12,
          name: "Syrup Hazelnut",
          image: "syrup_hazelnut-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 13,
          name: "Syrup Irish",
          image: "syrup_irish-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 14,
          name: "Syrup Kiwi",
          image: "syrup_kiwi-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 15,
          name: "Syrup Lemon",
          image: "syrup_lemon-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 16,
          name: "Syrup Lemongrass",
          image: "syrup_lemongrass-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 17,
          name: "Syrup Lychee",
          image: "syrup_lychee-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 18,
          name: "Syrup Manggo",
          image: "syrup_mango-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 19,
          name: "Syrup Mojito",
          image: "syrup_mojito_mint-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 20,
          name: "Syrup Pandan",
          image: "syrup_pandan-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 21,
          name: "Syrup Passion Fruit",
          image: "syrup_passion_fruit-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 22,
          name: "Syrup Peach",
          image: "syrup_peach-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 23,
          name: "Syrup Peppermint",
          image: "syrup_peppermint-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 24,
          name: "Syrup Strawberry",
          image: "syrup_strawberry-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 25,
          name: "Syrup Tiramisu",
          image: "syrup_tiramisu-removebg-preview.png",
          price: "97,000",
        },
        {
          id: 26,
          name: "Syrup Vanilla",
          image: "syrup_vanilla-removebg-preview.png",
          price: "97,000",
        },
      ],
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
.background {
  background: #fffbe8;
}
</style>
