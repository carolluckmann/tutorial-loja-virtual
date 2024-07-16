<script setup>
import { ref } from 'vue'
import ModalAddCategory from '@/components/ModalAddCategory.vue';

const showModal = ref(false)
</script>

<template>
  <h1>Adicionar Produtos</h1>
  <button @click="showModal = true">+</button>
    <modal-add-category v-if="showModal" @close="showModal = false"/>
</template>

<style scoped></style>
