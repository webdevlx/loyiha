<template>
  <div>
    <h1
      class="text-4xl lg:text-6xl text-slate-900 font-bold py-8 px-12 lg:px-32 lg:mt-16 text-center"
    >
      Rapidly build modern websites without ever leaving your HTML.
    </h1>
    <p class="text-xl font-medium text-gray-600 px-4 lg:px-64 text-center">
      A utility-first CSS framework packed with classes like
      <span class="text-sky-500 font-mono"> flex</span>,
      <span class="text-sky-500 font-mono"> pt-4</span>,
      <span class="text-sky-500 font-mono"> text-center </span>
      and
      <span class="text-sky-500 font-mono"> rotate-90</span>
      that can be composed to build any design, directly in your markup.
    </p>
    <div class="p-4 lg:px-96 lg:mt-12">
      <router-link
        to="/about"
        class="block text-center w-full bg-slate-900 text-white py-3 rounded-lg font-semibold"
        >Get started</router-link
      >
    </div>
  </div>
  <div class="p-4 text-3xl font-bold text-green-700">
    {{ $store.state.brand }}
  </div>
  <div class="p-4">
    <input class="w-full border-4 p-2" type="text" placeholder="Brand" v-model="$store.state.brand">
  </div>
</template>
