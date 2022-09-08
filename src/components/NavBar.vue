<template>
  <div class="bg-indigo-300 p-4 flex justify-center lg:justify-start gap-2">
    <router-link v-for="yollanma in yollanmalar" :key="yollanma" class="bg-indigo-500 text-white py-1 px-4 rounded-full font-bold border border-white hover:bg-white hover:text-indigo-500 hover:border-indigo-500 duration-300" :to="yollanma.manzil">{{ yollanma.nom }}</router-link>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      yollanmalar: [
        {
          manzil: '/',
          nom: 'Bosh sahifa'
        },
        {
          manzil: '/about',
          nom: 'Haqida'
        },
        {
          manzil: '/yordam',
          nom: 'Yordam'
        }
      ]
    }
  }
}
</script>