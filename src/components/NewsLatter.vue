<template>
  <div class="py-16 bg-white sm:py-24">
    <div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
      <div
        class="relative px-6 py-24 overflow-hidden bg-yellow-300 shadow-2xl isolate sm:rounded-3xl sm:px-24 xl:py-32">
        <h2
          class="max-w-2xl mx-auto text-3xl font-bold tracking-tight text-center text-yellow-900 sm:text-4xl">
          Get notified when we’re add new feature OR serious weather info
        </h2>
        <p
          class="max-w-xl mx-auto mt-2 text-lg leading-8 text-center text-black">
          Reprehenderit ad esse et non officia in nulla. Id proident tempor
          incididunt nostrud nulla et culpa.
        </p>
        <form class="flex max-w-md mx-auto mt-10 gap-x-4">
          <label for="email-address" class="sr-only">Email address</label>
          <input
            id="email-address"
            name="email"
            type="email"
            autocomplete="email"
            required
            class="min-w-0 flex-auto rounded-md border-0 bg-yellow-100 px-3.5 py-2 text-white shadow-sm ring-1 ring-inset ring-white/10 focus:ring-2 focus:ring-inset focus:ring-white sm:text-sm sm:leading-6"
            placeholder="Enter your email" />
          <button
            type="submit"
            class="flex-none rounded-md bg-yellow-800 px-3.5 py-2.5 text-sm font-semibold text-yellow-300 shadow-sm hover:bg-gray-100 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-white">
            Notify me
          </button>
        </form>
        <svg
          viewBox="0 0 1024 1024"
          class="absolute left-1/2 top-1/2 -z-10 h-[64rem] w-[64rem] -translate-x-1/2"
          aria-hidden="true">
          <circle
            cx="512"
            cy="512"
            r="512"
            fill="url(#759c1415-0410-454c-8f7c-9a820de03641)"
            fill-opacity="0.7" />
          <defs>
            <radialGradient
              id="759c1415-0410-454c-8f7c-9a820de03641"
              cx="0"
              cy="0"
              r="1"
              gradientUnits="userSpaceOnUse"
              gradientTransform="translate(512 512) rotate(90) scale(512)">
              <stop stop-color="#7775D6" />
              <stop offset="1" stop-color="#E935C1" stop-opacity="0" />
            </radialGradient>
          </defs>
        </svg>
      </div>
    </div>
  </div>
</template>
