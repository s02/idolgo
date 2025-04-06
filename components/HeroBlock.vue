<script setup></script>

<template>
  <div
    class="grid max-w-screen-xl pt-20 pb-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12 lg:pt-28"
  >
    <div class="lg:col-span-7">
      <h1
        class="font-extrabold max-w-2xl mb-4 text-4xl md:text-5xl xl:text-6xl"
      >
        <slot name="title"></slot>
      </h1>

      <p
        class="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl"
      >
        <slot name="text"></slot>
      </p>
    </div>
  </div>
</template>
