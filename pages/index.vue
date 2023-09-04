<template>
    <main>
        <Head>
            <Script defer data-domain="fadedow.com" src="https://plausible.io/js/plausible.js" />
        </Head>
        <div class="container mx-auto mt-4 flex justify-between">
            <NuxtLink to="/">
                <h2 class="ml-2 text-xl font-semibold">Fade<span class="text-green-400">Dow</span></h2>
            </NuxtLink>
            <div class="mr-2">
            <NuxtLink to="/blog" class=" bg-gray-500 hover:bg-gray-600 text-white py-2 px-4 rounded-sm mb-8">News</NuxtLink>
        </div>
    </div>
    <div class="container mx-auto px-4 mt-8 mb-8 text-md text-gray-200">
        <h3 class="mb-2 text-lg">Welcome to FadeDow. College Sports Betting.</h3>
        
        <p>Thanks for reading and if you'd like to reach out you can find me @adoughty on twitter. I'd love to hear from you! </p>
    </div>
    <Posts />
    <Footer />
</main>
</template>

<script setup lang="ts">
definePageMeta({
    colorMode: 'dark',
})

useSeoMeta({
  title: 'FadeDow Sports Betting',
  ogTitle: 'FadeDow Sports Betting Blog',
  description: 'College Football Sports Bettor',
  ogDescription: 'College Football Sports Bettor',
  ogImage: 'https://example.com/image.png',
  twitterCard: 'summary_large_image',
})

useHead({
  script: [
    {
      src: 'https://fadedow.com',
      tagPosition: 'head'
    }
  ]
})
</script>


<style>
body {
    /* background-color: #202122; */
    /* background-color: rgb(10 10 10); */
    background-color: rgb(23 23 23);
    color: #ffffff;
}

.dark-mode body {
    background-color: #091a28;
    color: #ebf4f1;
}

h1 {
    color: #ebf4f1;
    text-shadow: rgb(200, 200, 200) 1px 0 8px;
}

h2 {
    color: #ebf4f1;
}
</style>