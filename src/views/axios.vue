<template>
  <div id="app-container"></div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import axios from '../utils/axios.ts'

export default defineComponent({
  setup() {
    axios
      .get('/users/XPost')
      .then((response) => {
        console.log(response)
      })
      .catch((error) => {
        console.log(error)
      })
  }
})
</script>

<style scoped></style>
