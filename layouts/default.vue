<script setup>
useHead({
  scripts: [
    {
      type: 'text/javascript',
      src: 'https://www.googletagmanager.com/gtag/js?id=G-NQ5XEWSG9T',
      async: true,
      tagPosition: 'bodyClose'
    },
    {
      type: 'text/javascript',
      innerHTML: `
        window.dataLayer = window.dataLayer || []
        function gtag() {
          dataLayer.push(arguments)
        }
        gtag('js', new Date())

        gtag('config', 'G-NQ5XEWSG9T')
      `,
      tagPosition: 'bodyClose'
    }
  ],
  link: [
    {
      rel: 'preconnect',
      href: 'https://fonts.googleapis.com'
    },
    {
      rel: 'preconnect',
      href: 'https://fonts.gstatic.com',
      crossorigin: true
    },
    {
      rel: 'stylesheet',
      href: 'https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap'
    }
  ]
})
</script>
<template>
  <div class="bg-white px-4">
    <nav class="max-w-screen-xl mx-auto pt-2 flex gap-x-20">
      <NuxtLink to="/"><img class="logo" src="../assets/logo.jpg" /></NuxtLink>

      <ul class="flex items-center gap-x-12">
        <li>
          <NuxtLink to="/services">Services</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About Us</NuxtLink>
        </li>
      </ul>
    </nav>
    <slot></slot>
  </div>
</template>

<style lang="scss">
.logo {
  width: 50px;
}
</style>
