<script lang="ts" setup>
import {defineProps} from 'vue';
import {FontAwesomeIcon} from '@fortawesome/vue-fontawesome';


const props = defineProps({
  iconVariant: String,
  iconName: String,
});
</script>

<template>
  <font-awesome-icon :icon="[iconVariant, iconName]"/>

</template>

<style scoped>
/* Your component styles go here */
</style>
