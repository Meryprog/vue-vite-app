<template>
  <div class="min-h-screen bg-yellow-100 flex flex-col">
    <!-- Header -->
    <header class="p-4  flex items-center">
      <button class="text-gray-700 text-lg font-semibold hover:text-gray-900">
        &larr; Retour
      </button>
    </header>

    <!-- Main Content -->
    <main class="flex flex-1 justify-center items-center py-6">
      <form @submit.prevent="handleSubmit" class=" shadow-lg rounded-xl p-6 w-full max-w-md space-y-4">
        <!-- Image Placeholder -->
        <div class="flex flex-col items-center">
          <img
            src="/image.png"
            alt="Ajouter une image"
            class="w-24 h-24 rounded-lg mb-2 object-cover"
          />
          <button
            type="button"
            class="bg-green-500 text-white px-4 py-2 rounded-lg text-sm hover:bg-green-600"
          >
            Ajouter une image
          </button>
        </div>

        <!-- Form Fields -->
        <input
          type="text"
          placeholder="Nom de l'événement"
          v-model="form.nom"
          class="w-full p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          required
        />

        <div class="flex space-x-4">
          <input
            type="date"
            v-model="form.date"
            class="flex-1 p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
            required
          />
          <input
            type="time"
            v-model="form.heure"
            class="flex-1 p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
            required
          />
        </div>

        <input
          type="text"
          placeholder="Lieu de l'événement"
          v-model="form.lieu"
          class="w-full p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          required
        />

        <input
          type="number"
          placeholder="Nombre de participants"
          v-model="form.participants"
          class="w-full p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          required
        />

        <select
          v-model="form.type"
          class="w-full p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          required
        >
          <option value="" disabled selected>Type d'événement</option>
          <option value="Conférence">Conférence</option>
          <option value="Atelier">Atelier</option>
          <option value="Webinaire">Webinaire</option>
        </select>

        <div class="flex space-x-4">
          <input
            type="number"
            placeholder="Prix"
            v-model="form.prix"
            class="flex-1 p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          />
          <input
            type="time"
            v-model="form.duree"
            placeholder="Durée"
            class="flex-1 p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          />
        </div>

        <textarea
          placeholder="Description"
          v-model="form.description"
          class="w-full p-3 border rounded-lg text-gray-700 focus:outline-none focus:ring-2 focus:ring-green-500"
          rows="4"
          required
        ></textarea>

        <button
          type="submit"
          class="w-full bg-green-500 text-white py-3 rounded-lg text-lg font-semibold hover:bg-green-600"
        >
          Ajouter l'événement
        </button>
      </form>
    </main>
  </div>
</template>

<script>
export default {
  name: "AddEvent",
  data() {
    return {
      form: {
        nom: "",
        date: "",
        heure: "",
        lieu: "",
        participants: "",
        type: "",
        prix: "",
        duree: "",
        description: "",
      },
    };
  },
  methods: {
    handleSubmit() {
      console.log("Données du formulaire :", this.form);
      alert("Événement ajouté avec succès !");
    },
  },
};
</script>

<style scoped>
/* Aucune règle CSS supplémentaire grâce à Tailwind CSS */
</style>
