<script setup lang="ts">
import ItemTile from './ItemTile.vue'
</script>

<template>
    <div>
        <ItemTile>    
            <template #heading>Contact Details</template>
            <p>Email: alexander.g.dunphy@gmail.com</p>
            <p>Mobile: 0834741044</p>
            <p>LinkedIn: https://www.linkedin.com/in/alex-dunphy/</p>
            <p>Github: https://github.com/Dunphyal</p>
        </ItemTile>
        <ItemTile>    
            <template #heading>Education</template>
            <p>B.A.I. in Computer and Electronic Engineering</p>
            <p>Trinity College Dublin 2018 </p>
        </ItemTile>
        <ItemTile>    
            <template #heading>Education</template>
            <p>B.A.I. in Computer and Electronic Engineering</p>
            <p>Trinity College Dublin 2018 </p>
        </ItemTile>
    </div>
</template>

