<template>
  <section class="flex flex-col items-center bg-yellow-100 min-h-screen p-6">
    <!-- Vidéo de l'événement -->
    <div class="relative w-full max-w-md">
      <img src="/vodun.jpg" alt="\u00c9v\u00e9nement Vodun" class="rounded-lg w-full">
      <div class=" bg-black bg-opacity-50 absolute inset-0 flex justify-center items-center">
        <button class=" text-red-600 text-4xl rounded-full p-28">
          <img src="/logosf.png" alt="">
        </button>
        <!--  -->
      </div>
    </div>

    <!-- Informations sur l'\u00e9v\u00e9nement -->
    <div class="flex items-center justify-between mt-4 w-full max-w-md">
      <img src="/eventlogo.jpeg" alt="Logo" class="w-12 h-12 rounded-full">
      <div class="flex-1 mx-4">
        <h3 class="text-lg font-bold">Vodun Days 10 Janvier 2024</h3>
        <p class="text-gray-500 text-sm">500 vues . Il y a 11 mois</p>
      </div>
      <div class="flex items-center">
        <span class="text-gray-700 text-sm">20 likes</span>
        <img src="/Like.png" alt="Like" class="w-5 h-5 ml-2">
      </div>
    </div>

    <!-- Chats en direct -->
    <div class="mt-6 w-full max-w-md">
      <h4 class="text-lg font-semibold mb-2">Chats en direct</h4>
      <ul class="space-y-2">
        <li class="flex items-center">
          <span class="bg-orange-500 w-3 h-3 rounded-full mr-2"></span> Trop top
        </li>
        <li class="flex items-center">
          <span class="bg-green-500 w-3 h-3 rounded-full mr-2"></span> Wouahhhhhhh
        </li>
        <li class="flex items-center">
          <span class="bg-green-500 w-3 h-3 rounded-full mr-2"></span> Spectaculaire
        </li>
        <li class="flex items-center">
          <span class="bg-orange-500 w-3 h-3 rounded-full mr-2"></span> C'est intriguant
        </li>
        <li class="flex items-center">
          <span class="bg-green-500 w-3 h-3 rounded-full mr-2"></span> C'est le Bénin qui gagne
        </li>
        <li class="flex items-center">
          <span class="bg-black w-3 h-3 rounded-full mr-2"></span> Fière de la culture Béninoise
        </li>
        <li class="flex items-center">
          <span class="bg-green-500 w-3 h-3 rounded-full mr-2"></span> Wouahhhhhhh
        </li>
        <li class="flex items-center">
          <span class="bg-green-500 w-3 h-3 rounded-full mr-2"></span> Trop top
        </li>
      </ul>
    </div>

    <!-- Bouton de commentaire -->
    <div class="mt-6">
      <input class="px-6 py-3 border border-gray-300 rounded-full bg-white hover:bg-gray-100 text-gray-700"
      placeholder="Mettre un commentaire">
    </div>
  </section>
</template>

<script>
export default {
  name: "OneEvent",
};
</script>

<style scoped>
</style>
