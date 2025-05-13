<script setup>
const { description } = useAppConfig()
</script>

<template>
  <main
    class="grid py-8 bg-gradient-to-br from-neutral-50 dark:from-neutral-900 via-neutral-50 to-amber-100 ring-1 ring-foreground/5 rounded-3xl p-6 lg:grid-cols-2 place-items-center md:py-12"
  >
    <div class="w-full ps-14">
      <h1
        class="text-5xl font-bold lg:text-6xl xl:text-7xl lg:tracking-tight xl:tracking-tighter"
      >
        Ciutkan tautan mu
      </h1>
      <p class="max-w-xl mt-4 text-lg text-neutral-600">
        {{ description }}
      </p>
      <div class="flex flex-col gap-3 mt-6 sm:flex-row">
        <HomeLink
          href="/dashboard"
          class="flex rounded-full bg-amber-400 hover:bg-amber-600 text-amber-900 hover:text-amber-100 transition-all duration-150 ease-linear text-3xl w-auto px-8 h-20 object-center font-semibold p-20 items-center justify-center gap-1"
          rel="noopener"
        >
          Mulai mengerucutkan
        </HomeLink>
      </div>
    </div>
    <img src="@/assets/images/hero.webp" alt="Hero image" class="w-60 translate-x-40 md:flex hidden">
  </main>
</template>
