<template>
  <div>
    <h1 class="extra-bold text-3xl text-center mb-6">Home</h1>
<p>name in store {{name}}</p>
  </div>
</template>

<script setup>
import {computed} from 'vue'
import {useStore} from 'vuex';

const store =useStore();
const name = computed(() => store.state.user.name)

</script>

<style lang="scss" scoped>

</style>