<script lang="ts" setup>

import SingleSocial from "@/components/social/SingleSocial.vue";

const socials = [
  {
    title: "Social 1",
    description: "This is the first social",
    Due: 10 / 10 / 2021,
    isChecked: false,
  },
  {
    title: "Social 2",
    description: "This is the second social",
    Due: 9 / 10 / 2021,
    isChecked: false,
  },
  {
    title: "Social 3",
    description: "This is the third social",
    Due: 10 / 10 / 2021,
    isChecked: true,
  },
  // Add more socials as needed
];
</script>

<template>
  <h2>Socials</h2>
  <div class="grid grid-cols-6 gap-4">
    <div>
      <SingleSocial social="facebook"/>
    </div>
  </div>
</template>

<style scoped>

</style>