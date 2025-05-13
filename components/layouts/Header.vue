<script setup>
const { title } = useAppConfig()
</script>

<template>
  <section class="pb-6">
    <nav class="container relative z-50 h-24 select-none">
      <div
        class="container relative flex flex-wrap items-center justify-between h-24 px-0 mx-auto overflow-hidden font-medium md:overflow-visible lg:justify-center"
      >
        <div class="flex w-full items-center justify-start h-full pr-4">
          <a
            href="/"
            :title="title"
            class="flex items-center w-full py-4 space-x-2 text-xl font-black text-gray-900 dark:text-gray-100 md:py-0"
          >
            <span
              class="flex items-center justify-center w-8 h-8 rounded-full"
            >
              <img
                src="/sink.png"
                :alt="title"
                class="w-full h-full rounded-full"
              >
            </span>
            <span class="mx-2">{{ title }}</span>
          </a>
          <SwitchTheme />
        </div>
      </div>
    </nav>
  </section>
</template>
