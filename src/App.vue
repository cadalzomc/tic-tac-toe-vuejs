<script setup lang="ts">
import Board from "./components/Board/Board.vue"
import PlayerX from "@/components/Record/Player.X.vue"
import PlayerO from "@/components/Record/Player.O.vue"
import Draw from "@/components/Record/Draw.vue"
</script>

<template>
  <main class="flex w-screen h-screen justify-center items-center overflow-auto">
    <div class="py-8 px-8 text-center max-sm:w-full max-sm:px-4">
      <div class="block w-full text-center">
        <Board />
        <div class="grid grid-cols-3 justify-between gap-3 mt-2">
          <PlayerX />
          <Draw />
          <PlayerO />
        </div>
      </div>
    </div>
  </main>
</template>
