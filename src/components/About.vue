<template>
  <a name="about-us">
    <div class="bg-white py-12">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl lg:max-w-none">
          <div class="text-center">
            <h2
              class="text-balance text-4xl font-semibold tracking-tight text-gray-900 sm:text-5xl"
            >
              About Us
            </h2>
            <p class="mt-4 text-lg/8 text-gray-600">
              We are a locally-owned and operated plumbing business dedicated to serving our
              community with reliable, efficient, and affordable plumbing solutions.
            </p>
            <p class="mt-4 text-lg/8 text-gray-600">
              At Nova Plumbing, we understand how important it is to have a trustworthy partner for
              all your plumbing needs. Whether you're dealing with a leaky faucet, a clogged drain,
              or a major renovation project, our skilled team is here to provide expert service
              tailored to your needs.
            </p>
          </div>
          <dl
            class="mt-16 grid grid-cols-1 gap-0.5 overflow-hidden rounded-2xl text-center lg:grid-cols-2"
          >
            <div v-for="stat in stats" :key="stat.id" class="flex flex-col bg-gray-400/5 p-8">
              <dt class="text-sm/6 font-semibold text-gray-600">{{ stat.name }}</dt>
              <dd class="order-first text-3xl font-semibold tracking-tight text-gray-900">
                {{ stat.value }}
              </dd>
            </div>
          </dl>
        </div>
      </div>
    </div>
  </a>
</template>

<script setup>
const stats = [
  { id: 1, name: 'Phone Number', value: '1-801-980-1311' },
  { id: 2, name: 'Email', value: 'nate.rencher@gmail.com' },
]
</script>
