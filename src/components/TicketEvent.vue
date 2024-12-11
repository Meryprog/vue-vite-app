<template>
  <div class="flex justify-center items-center min-h-screen bg-yellow-200">
    <div class="container bg-white rounded-2xl shadow-lg overflow-hidden max-w-md w-full">
      <!-- Barre de titre -->
      <header class="flex items-center p-4 bg-yellow-300">
        <RouterLink to="/tickets">
          <button class="text-lg font-semibold text-gray-700 hover:text-gray-900">&larr; Tickets</button>
        </RouterLink>
      </header>

      <!-- Ticket principal -->
      <main class="p-6">
        <div class="ticket-card bg-white rounded-lg shadow-md p-4">
          <h3 class="text-xl font-bold mb-2">Nom de l'évènement:</h3>
          <p class="text-gray-700 text-lg mb-4">Afro Music Festival 2024</p>

          <div class="grid grid-cols-2 gap-4 mb-4">
            <div>
              <p class="text-sm font-semibold">Date et heure :</p>
              <p class="text-gray-600">12/12/2024<br>17h15</p>
            </div>
            <div>
              <p class="text-sm font-semibold">Lieu :</p>
              <p class="text-gray-600">Stade XYZ</p>
            </div>
          </div>

          <div class="grid grid-cols-2 gap-4 mb-4">
            <div>
              <p class="text-sm font-semibold">Numéro de ticket :</p>
              <p class="text-gray-600">1452678873578</p>
            </div>
            <div>
              <p class="text-sm font-semibold">Nom du détenteur :</p>
              <p class="text-gray-600">MdiGial</p>
            </div>
          </div>

          <div class="grid grid-cols-2 gap-4 mb-4">
            <div>
              <p class="text-sm font-semibold">Type de billet :</p>
              <p class="text-gray-600">VIP</p>
            </div>
            <div>
              <p class="text-sm font-semibold">Prix :</p>
              <p class="text-gray-600">150000 Fcfa</p>
            </div>
          </div>

          <div class="text-center mt-4">
            <img src="/code_bar.png" alt="Code-barre" class="w-48 mx-auto">
          </div>
        </div>

        <!-- QR Code -->
        <div class="qr-section bg-green-600 text-white rounded-lg shadow-md mt-6 p-4 text-center">
          <p class="text-lg font-semibold">Nom du détenteur : MdiGial</p>
          <p class="text-lg">Prix : 150000 Fcfa</p>
          <!-- <div class="mt-4">
            <img src="/qrcode.png" alt="QR Code" class="w-24 h-24 mx-auto">
          </div> -->
        </div>
      </main>
    </div>
  </div>
</template>

<script>
export default {
  name: "TicketEvent",
};
</script>

<style scoped>
</style>
