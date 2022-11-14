<template>
  <div class="flex-row flex py-2">
    <i class="pt-1 mr-2">
      <slot name="icon"></slot>
    </i>
    <div class="flex flex-col w-full">
      <h3 class="font-mono flex gap-2 font-black text-lg">
        <slot name="heading"></slot>
      </h3>
      <div class="text-justify">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>
