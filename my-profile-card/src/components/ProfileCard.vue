<script setup>
defineProps([
  "name",
  "subheading",
  "background",
  "profileimg",
  "followers",
  "following",
  "projects",
  "facebook",
  "instagram",
  "linkedin",
]);
</script>

<template>
  <div
    class="bg-white shadow-lg rounded-2xl min-[32opx] overflow-hidden text-center"
  >
    <div
      class="relative min-h-32 bg-cover bg-center"
      :style="'background-image: url(' + background + ')'"
    >
      <img
        :src="profileimg"
        alt="Profile Image"
        class="inline-block w-32 h-32 rounded-full object-center object-cover border-6 border-white absolute top-full left-1/2 transform -translate-1/2"
      />
    </div>

    <div class="px-6 pt-20 pb-6">
      <h2 class="font-bold text-gray-800 text-2xl mb-2">{{ name }}</h2>

      <h3 class="text-gray-600 text-lg">{{ subheading }}</h3>
    </div>
    <div class="flex justify-center gap-4 pb-2">
      <a
        v-if="facebook"
        :href="facebook"
        target="_blank"
        class="text-blue-600 hover:text-blue-800 transition-colors"
      >
        <svg class="w-6 h-6 fill-current" viewBox="0 0 24 24">
          <path
            d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"
          />
        </svg>
      </a>

      <a
        v-if="instagram"
        :href="instagram"
        target="_blank"
        class="text-pink-600 hover:text-pink-800 transition-colors"
      >
        <svg class="w-6 h-6 fill-current" viewBox="0 0 24 24">
          <path
            d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"
          />
        </svg>
      </a>

      <a
        v-if="linkedin"
        :href="linkedin"
        target="_blank"
        class="text-blue-700 hover:text-blue-900 transition-colors"
      >
        <svg class="w-6 h-6 fill-current" viewBox="0 0 24 24">
          <path
            d="M4.98 3.5c0 1.381-1.11 2.5-2.48 2.5s-2.48-1.119-2.48-2.5c0-1.38 1.11-2.5 2.48-2.5s2.48 1.12 2.48 2.5zm.02 4.5h-5v16h5v-16zm7.982 0h-4.968v16h4.969v-8.399c0-4.67 6.029-5.052 6.029 0v8.399h4.988v-10.131c0-7.88-8.922-7.593-11.018-3.714v-2.155z"
          />
        </svg>
      </a>
    </div>

    <div
      class="p-6 border-t border-gray-200 flex items-center justify-center gap-6"
    >
      <div>
        <h4 class="text-gray-600 text-sm">Followers</h4>
        <p class="font-bold text-gray-800 text-2xl">{{ followers }}</p>
      </div>

      <div>
        <h4 class="text-gray-600 text-sm">Following</h4>
        <p class="font-bold text-gray-800 text-2xl">{{ following }}</p>
      </div>

      <div>
        <h4 class="text-gray-600 text-sm">Projects</h4>
        <p class="font-bold text-gray-800 text-2xl">{{ projects }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
