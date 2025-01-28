<template>
  <a name="services">
    <div class="overflow-hidden bg-white py-24 sm:py-24">
      <div class="mx-auto max-w-7xl px-6 lg:px-20">
        <div
          class="mx-auto grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:gap-y-20 lg:mx-0 lg:max-w-none lg:grid-cols-2"
        >
          <div class="lg:ml-auto lg:pl-4 lg:pt-4">
            <div class="lg:max-w-lg">
              <p
                class="mt-2 text-pretty text-4xl font-semibold tracking-tight text-gray-900 sm:text-6xl"
              >
                Services
              </p>
              <dl class="mt-12 max-w-xl space-y-8 text-base/7 text-gray-600 lg:max-w-none">
                <div v-for="feature in features" :key="feature.name" class="relative pl-9">
                  <dt class="inline font-semibold text-gray-900 sm:text-3xl">
                    <component
                      :is="feature.icon"
                      class="absolute left-0 top-1 size-8 text-nova-blue"
                      aria-hidden="true"
                    />
                    {{ feature.name }}
                  </dt>
                  {{ ' ' }}
                  <dd class="inline">{{ feature.description }}</dd>
                </div>
              </dl>
            </div>
          </div>
          <div class="flex items-start justify-end lg:order-first">
            <img
              src="https://nova-plumbing.s3.us-east-2.amazonaws.com/IMG_3241_VSCO.JPG"
              alt="Nova Plumbing Team"
              class="rounded-xl shadow-xl ring-1 ring-gray-400/10"
              width="2432"
              height="1442"
            />
          </div>
        </div>
      </div>
    </div>
  </a>
</template>

<script setup>
import { ShieldCheckIcon, LockClosedIcon, ServerIcon } from '@heroicons/vue/24/outline'

const features = [
  {
    name: 'Water Heaters',
    icon: ShieldCheckIcon,
  },
  {
    name: 'Water Softener Installation',
    icon: ShieldCheckIcon,
  },
  {
    name: 'General Repairs',
    icon: ShieldCheckIcon,
  },
  {
    name: 'Plumbing Upgrades',
    icon: ShieldCheckIcon,
  },
  {
    name: 'Basement Remodel',
    icon: ShieldCheckIcon,
  },
  {
    name: 'New Construction',
    icon: ShieldCheckIcon,
  },
]
</script>
