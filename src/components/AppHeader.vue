<template>
  <div>
    <div class="p-4">
      <nav
        class="container px-4 py-5 mx-auto lg:flex lg:justify-between lg:items-center lg:px-6 xl:px-12"
      >
        <div class="flex items-center justify-between">
          <router-link
            to="/"
            class="text-xl font-bold text-gray-800 lg:text-2xl hover:text-blue-400"
            ><img
              src="../assets/images/logo/Genova_Logo_no_bg.png"
              alt="Logo Genova"
              height="100"
              width="100"
            />
          </router-link>
          <!-- Mobile menu button -->
          <div @click="showMenu = !showMenu" class="flex lg:hidden">
            <button
              type="button"
              class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400"
            >
              <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                <path
                  fill-rule="evenodd"
                  d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
                ></path>
              </svg>
            </button>
          </div>
        </div>

        <div class="flex justify-center lg:order-2">
          <div :class="showMenu ? 'block' : 'hidden'" class="relative lg:block">
            <div
              class="flex absolute inset-y-0 left-0 items-center pl-3 pointer-events-none"
            >
              <svg
                class="w-5 h-5 text-gray-500"
                aria-hidden="true"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
                  clip-rule="evenodd"
                ></path>
              </svg>
              <span class="sr-only">Search icon</span>
            </div>
            <input
              type="text"
              id="search-navbar"
              class="block p-2 pl-10 w-full text-gray-900 bg-gray-50 rounded-lg border border-gray-300 sm:text-sm focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500"
              placeholder="Search..."
            />
          </div>
        </div>

        <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
        <ul
          :class="showMenu ? 'block' : 'hidden'"
          class="flex-col mt-8 space-y-4 lg:flex lg:space-y-0 lg:flex-row lg:items-center lg:space-x-10 lg:mt-0 lg:order-1"
        >
          <li class="text-base font-semibold text-gray-800 hover:text-blue-400">
            <router-link to="/products">Product</router-link>
          </li>
          <li class="text-base font-semibold text-gray-800 hover:text-blue-400">
            <router-link to="/recipe">Recipe</router-link>
          </li>
          <li class="text-base font-semibold text-gray-800 hover:text-blue-400">
            <router-link to="/about">About Us</router-link>
          </li>
          <li class="text-base font-semibold text-gray-800 hover:text-blue-400">
            <router-link to="/contact">Contact</router-link>
          </li>
          <li class="text-base font-semibold text-gray-800 hover:text-blue-400">
            <router-link @click="dropdownClose" to="/location"
              >Location</router-link
            >
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showMenu: false,
      // dropdown: false,
      // isOpen: false,
      // theme: "",
      // modal: false,
    };
  },
  toggleNav: function () {
    this.showMenu = !this.showMenu;
  },
  // dropdownClose() {
  //   this.showMenu = !this.showMenu;
  // },
};
</script>
