<script lang="ts" setup>

import Icon from "@/components/icons/icon.vue";

const props = defineProps({social: String})
const fbUrl = "https://www.facebook.com/ismail.nyzar.1/";
</script>

<template>
  <!--  variables should be saved-->
  <a :href=fbUrl>
    <div class="grid grid-cols-6 gap-4">
      <icon icon-variant="fab" iconName="facebook"></icon>
      {{ social }}
    </div>
  </a>
</template>

<style scoped>

</style>