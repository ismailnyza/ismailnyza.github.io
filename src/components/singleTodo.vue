<script lang="ts" setup>
import {defineProps} from 'vue'

const props = defineProps({title: String, description: String, Due: Date, isChecked: Boolean})
let isChecked = false
if (props.isChecked) {
  isChecked = true
}
</script>

<template>
  <div class="grid grid-cols-6 gap-4">
    <div>{{ title }}</div>
    <p>{{ description }}</p>
    <p>{{ Due }}</p>
    <!--  add fields like due date location progress and stuff-->
    <input v-model="isChecked" type="checkbox">
  </div>
</template>

<style scoped>

</style>