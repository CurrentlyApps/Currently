<template>
  <div class="flex-row flex bg-zinc-800 p-10 w-96 m-5 md:m-10 shadow-2xl rounded-lg ">
    <div class="flex flex-col w-full">
      <h3 :class="`${getRandomColor()} font-mono flex gap-2 font-black text-lg text-zinc-100`">
        <slot name="icon"></slot>
        <slot name="heading"></slot>
      </h3>
      <div class="text-justify text-zinc-100">
        <slot></slot>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">

const randomColors = [
  'text-amber-400',
  'text-red-400',
  'text-blue-400',
  'text-green-400',
  'text-purple-400',
  'text-pink-400',
  'text-yellow-400',
  'text-indigo-400',
  'text-teal-400',
  'text-cyan-400',
  'text-orange-400',
  'text-lime-400',

]

function getRandomColor (){
  return randomColors[Math.floor(Math.random() * randomColors.length)]
}

</script>
<style scoped>
</style>
