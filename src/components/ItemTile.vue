<script setup lang="ts">
import { ref } from 'vue';

    let additionalInfo = ref('')

    function addInfo() {
        additionalInfo.value ? additionalInfo.value = '' : additionalInfo.value = 'new string'
    }

</script>

<template>
  <div class="item">
    <div class="details">
        <div class="title">
            <h3>
                <slot name="heading"></slot>
            </h3>
            <div @click="addInfo">X</div>
        </div>
      <slot></slot>
      <div>{{additionalInfo}}</div>
    </div>
  </div>
</template>

<style scoped>
    .item {
        margin-top: 2rem;
        padding: 2rem;
        background-color:darkslateblue;
        color:goldenrod;
        border-radius: 2rem;
    }

    .title {
        display: flex;
        justify-content: space-between;
    }

    h3 {
        font-size: 1.2rem;
        font-weight: bold;
        margin-bottom: 0.4rem;
    }
</style>