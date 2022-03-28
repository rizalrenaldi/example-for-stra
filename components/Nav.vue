<template>
  <div class="fixed inset-0 w-full h-16 bg-transparent">
    <div
      class="container flex items-center justify-between h-full px-4 mx-auto"
    >
      <div></div>
      <div class="dark:text-white text-zinc-900">
        <button
          v-if="$colorMode.preference === 'light'"
          @click="$colorMode.preference = 'dark'"
        >
          <svg
            class="w-6"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g fill="none" class="signal-icon-wrapper" stroke="none">
              <path
                d="M21.25 12.114a6.75 6.75 0 0 1-9.363-9.363 9.25 9.25 0 1 0 9.362 9.363z"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </g>
          </svg>
        </button>
        <button
          v-if="$colorMode.preference === 'dark'"
          @click="$colorMode.preference = 'light'"
        >
          <svg
            class="w-6"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g fill="none" class="signal-icon-wrapper" stroke="none">
              <path
                d="M20.25 3.75l-2.5 2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M3.75 3.75l2.5 2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M20.25 20.25l-2.5-2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M3.75 20.25l2.5-2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M12 2.75v2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M12 21.25v-2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M21.25 12h-2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M2.75 12h2.5"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
              <path
                d="M16.25 12a4.25 4.25 0 1 1-8.5 0 4.25 4.25 0 0 1 8.5 0z"
                stroke="currentColor"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </g>
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>