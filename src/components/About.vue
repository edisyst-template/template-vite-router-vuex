<template>
  <h1 class="font-bold text-2xl">
    About {{ name }}
  </h1>
  <span @click="router.push('/')">Torna alla home</span>
</template>

<script setup>
import { computed } from 'vue'
import { useStore } from 'vuex'
import { useRouter } from 'vue-router'

const router = useRouter()
const store = useStore()

const name = computed(() => {
  return store.state.user.name
})

</script>
