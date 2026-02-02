<script setup>
import ProfileCard from "./components/ProfileCard.vue";
</script>

<template>
  <div
    class="flex items-center justify-center gap-8 min-h-screen bg-gradient-to-br from-green-400 to-sky-400"
  >
    <ProfileCard
      name="Rapeepong Naksan"
      subheading="Student, 20, BKK"
      background="./src/assets/background.jpg"
      profileimg="./src/assets/profile.png"
      followers="58k"
      following="512"
      projects="10+"
      facebook="https://facebook.com"
      instagram="https://instagram.com"
      linkedin="https://linkedin.com"
    />

    <ProfileCard
      name="Jane Doe"
      subheading="Designer, 24, NYC"
      background="./src/assets/background.jpg"
      profileimg="./src/assets/profile.png"
      followers="12k"
      following="150"
      projects="5"
      facebook="https://facebook.com"
      instagram="https://instagram.com"
      linkedin="https://linkedin.com"
    />

    <ProfileCard
      name="John Smith"
      subheading="Developer, 28, LDN"
      background="./src/assets/background.jpg"
      profileimg="./src/assets/profile.png"
      followers="8k"
      following="300"
      projects="25+"
      facebook="https://facebook.com"
      instagram="https://instagram.com"
      linkedin="https://linkedin.com"
    />
  </div>
</template>

<style scoped></style>
