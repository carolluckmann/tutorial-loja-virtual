<script setup>
const emit = defineEmits(['close']);

</script>

<template>
    <div class="modal">
        <div class="modal-content">
            <button @click="$emit('close')" class="btn-close">
                <i class="mdi mdi-close" />
            </button>
        </div>
    </div>
<template/>

<style scoped>
.modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 100;
}

.modal-content {
  background-color: white;
  padding: 2rem;
  border-radius: 10px;
  width: 30%;
}

.btn-close {
  background-color: #0a2668;
  color: white;
  border: none;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  cursor: pointer;
}

</style>