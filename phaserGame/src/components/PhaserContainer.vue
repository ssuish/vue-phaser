<template>
    <div id="game">
        <ion-button v-if="showButton" @click="handleClickStart">Start</ion-button>
    </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue'
import { IonButton } from '@ionic/vue';
import { Game } from 'phaser';

const showButton = ref(true)

function launch() {

}

function handleClickStart() {
    showButton.value = false
    launch()
}

</script>

<style lang="css" scoped>
#game {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
}
</style>