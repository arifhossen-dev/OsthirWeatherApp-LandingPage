<script setup>
const pricingData = {
  hobby: {
    price: 19,
    features: [
      '25 products',
      'Up to 10,000 subscribers',
      'Advanced analytics',
      '24-hour support response time',
    ]
  },
  enterprise: {
    price: 49,
    features: [
      'Unlimited products',
      'Unlimited subscribers',
      'Advanced analytics',
      'Dedicated support representative',
      'Marketing automations',
      'Custom integrations',
    ]
  }
}
</script>
<template>
  <section id="pricing" class="relative px-6 py-24 bg-white isolate sm:py-32 lg:px-8">
    <div class="absolute inset-x-0 overflow-hidden -top-3 -z-10 transform-gpu px-36 blur-3xl" aria-hidden="true">
      <div class="mx-auto aspect-[1155/678] w-[72.1875rem] bg-gradient-to-tr from-[#ff80b5] to-[#9089fc] opacity-30"
        style="
          clip-path: polygon(
            74.1% 44.1%,
            100% 61.6%,
            97.5% 26.9%,
            85.5% 0.1%,
            80.7% 2%,
            72.5% 32.5%,
            60.2% 62.4%,
            52.4% 68.1%,
            47.5% 58.3%,
            45.2% 34.5%,
            27.5% 76.7%,
            0.1% 64.9%,
            17.9% 100%,
            27.6% 76.8%,
            76.1% 97.7%,
            74.1% 44.1%
          );
        "></div>
    </div>
    <div class="max-w-2xl mx-auto text-center lg:max-w-4xl">
      <h2 class="text-base font-semibold leading-7 text-indigo-600">Pricing</h2>
      <p class="mt-2 text-4xl font-bold tracking-tight text-gray-900 sm:text-5xl">
        The right price for you, whoever you are
      </p>
    </div>
    <p class="max-w-2xl mx-auto mt-6 text-lg leading-8 text-center text-gray-600">
      Qui iusto aut est earum eos quae. Eligendi est at nam aliquid ad quo
      reprehenderit in aliquid fugiat dolorum voluptatibus.
    </p>
    <div
      class="grid items-center max-w-lg grid-cols-1 mx-auto mt-16 gap-y-6 sm:mt-20 sm:gap-y-0 lg:max-w-4xl lg:grid-cols-2">
      <div
        class="p-8 rounded-3xl ring-1 ring-yellow-300 sm:p-10 bg-white/60 sm:mx-8 lg:mx-0 rounded-t-3xl sm:rounded-b-none lg:rounded-tr-none lg:rounded-bl-3xl">
        <h3 id="tier-hobby" class="text-base font-semibold leading-7 text-yellow-600">
          Hobby
        </h3>
        <p class="flex items-baseline mt-4 gap-x-2">
          <span class="text-5xl font-bold tracking-tight text-yellow-400">${{ pricingData.hobby.price }}</span>
          <span class="text-base text-black">/month</span>
        </p>
        <p class="mt-6 text-base leading-7 text-black">
          The perfect plan if you&#039;re just getting started with our product.
        </p>
        <ul role="list" class="mt-8 space-y-3 text-sm leading-6 text-gray-600 sm:mt-10">
          <template v-for="feature in pricingData.hobby.features">

            <li class="flex text-black gap-x-3">
              <svg class="flex-none w-5 h-6 text-red-600" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                <path fill-rule="evenodd"
                  d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                  clip-rule="evenodd" />
              </svg>
              {{ feature }}
            </li>
          </template>
        </ul>
        <a href="#" aria-describedby="tier-hobby"
          class="mt-8 block rounded-md py-2.5 px-3.5 text-center text-sm font-semibold focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 sm:mt-10 text-yellow-600 ring-1 ring-inset ring-yellow-500 hover:ring-yellow-300 focus-visible:outline-yellow-600">
          Get started today
        </a>
      </div>
      <div
        class="relative p-8 text-yellow-700 border-8 border-yellow-200 shadow-2xl rounded-3xl ring-1 ring-gray-900/10 sm:p-10">
        <h3 id="tier-enterprise" class="text-base font-semibold leading-7">
          Enterprise
        </h3>
        <p class="flex items-baseline mt-4 gap-x-2">
          <span class="text-5xl font-bold tracking-tight">${{ pricingData.enterprise.price }}</span>
          <span class="text-base">/month</span>
        </p>
        <p class="mt-6 text-base leading-7">
          Dedicated support and infrastructure for your company.
        </p>
        <ul role="list" class="mt-8 space-y-3 text-sm leading-6 text-gray-300 sm:mt-10">
          <template v-for="feature in pricingData.enterprise.features">
            <li class="flex text-yellow-700 gap-x-3">
              <svg class="flex-none w-5 h-6 text-red-500" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                <path fill-rule="evenodd"
                  d="M16.704 4.153a.75.75 0 01.143 1.052l-8 10.5a.75.75 0 01-1.127.075l-4.5-4.5a.75.75 0 011.06-1.06l3.894 3.893 7.48-9.817a.75.75 0 011.05-.143z"
                  clip-rule="evenodd" />
              </svg>
              {{ feature }}
            </li>
          </template>
        </ul>
        <a href="#" aria-describedby="tier-enterprise"
          class="mt-8 block rounded-md py-2.5 px-3.5 text-center text-sm font-semibold focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 sm:mt-10 bg-yellow-500 text-white shadow-sm hover:bg-yellow-600 focus-visible:outline-yellow-700">Get
          started today</a>
      </div>
    </div>
  </section>
</template>
