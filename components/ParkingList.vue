<template>
  <div class="container px-6 py-10 mx-auto">
    <div
      class="p-4 w-full bg-white rounded-lg border shadow-md sm:p-8 dark:bg-gray-800 dark:border-gray-700"
    >
      <div class="flex justify-between items-center mb-4">
        <h3 class="text-xl font-bold leading-none text-gray-900 dark:text-white">
          Top 3 lowest priced parkings
        </h3>
      </div>
      <div class="flow-root">
        <ul role="list" class="divide-y divide-gray-200 dark:divide-gray-700">
          <li v-for="(parking, i) in parkings" :key="parking.name" class="py-3 sm:py-4">
            <div class="flex items-center space-x-4">
              <div class="flex-1 min-w-0">
                <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
                  parkings {{ i + 1 }} : {{ parking.name }}
                </p>
                <p class="text-sm text-gray-500 truncate dark:text-gray-400">
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur
                  magnam optio non repellat vitae corrupti fugiat iusto ab corporis
                  perspiciatis!
                </p>
              </div>
              <div
                class="flex justify-center text-center items-center text-base font-semibold text-gray-900 dark:text-white"
              >
                EUR
                <br />
                {{ parking.price }}
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    parkings: {
      type: Array,
      default() {
        return [];
      },
    },
  },
};
</script>
