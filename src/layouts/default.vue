<template>
  <div class="flex h-screen overflow-hidden text-neutral-900 bg-neutral-50">
    <div
      class="flex-col flex-none hidden w-56 h-full min-h-0 py-3 space-y-3 bg-white border-r shadow border-neutral-200 sm:flex"
    >
      <a href="/" class="flex-none mx-auto text-4xl">
        <Logo />
      </a>
      <div class="flex-grow py-6 overflow-y-auto">
        <Chapter title="Introduction" subtitle="Understanding Tailwind CSS">
          <router-link to="/get-started" class="flex items-center p-2 space-x-1">
            <carbon-rocket class="w-5 h-5" />
            <span>Get started</span>
          </router-link>
        </Chapter>
        <Chapter title="Chapter_1" subtitle="Basic usage of Tailwind CSS">
          <router-link to="/basic-configuration" class="flex items-center p-2 space-x-1">
            <carbon-audio-console class="w-5 h-5" />
            <span>Basic configuration</span>
          </router-link>
        </Chapter>
      </div>
      <div class="flex-none mx-auto">
        <a
          href="https://github.com/ethylon/FAQwind"
          class="flex items-center space-x-1"
          target="_blank"
          actions
        >
          <span class="text-sm font-semibold">GitHub</span>
          <carbon-logo-github class="w-6 h-6" />
        </a>
      </div>
    </div>
    <main class="flex-grow overflow-y-auto">
      <div class="container flex flex-col pt-16 mx-auto">
        <router-view></router-view>
      </div>
    </main>
  </div>
</template>
