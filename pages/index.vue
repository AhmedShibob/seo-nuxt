<template>
  <div>
    <BaseHeader />

    <ParkingLIst />

    <section class="container px-6 py-10 mx-auto">
      <h1
        class="text-3xl font-semibold text-gray-800 capitalize lg:text-4xl dark:text-white"
      >
        Compare Airport Parking Lots
      </h1>

      <p class="mt-3 text-sm text-gray-500 dark:text-gray-300 md:text-sm">
        Compare parking spaces and prices at all major airports in Europe
      </p>
    </section>

    <section class="container px-6 py-10 mx-auto">
      <div class="container px-5 py-24 mx-auto">
        <div class="text-center mb-20">
          <h1
            class="sm:text-3xl text-2xl font-medium text-center title-font text-gray-900 mb-4"
          >
            Frequently Asked Question
          </h1>
          <p class="text-base leading-relaxed xl:w-2/4 lg:w-3/4 mx-auto">
            The most common questions about how our business works and what can do for
            you.
          </p>
        </div>
        <div class="flex flex-wrap lg:w-4/5 sm:mx-auto sm:mb-2 -mx-2">
          <div class="w-full lg:w-1/2 px-4 py-2">
            <details v-for="item in 3" :key="item" class="mb-4">
              <summary class="font-semibold bg-gray-200 rounded-md py-2 px-4">
                What do our customers say about us?
              </summary>

              <span>
                In the end it’s all about the customers opinion. We are very pleased with
                the good appreciation of our customers. Our service is valued on average
                with an 8,5/10 based on 5797 rating. We are proud of the high rating we
                have received.
              </span>
            </details>
          </div>
          <div class="w-full lg:w-1/2 px-4 py-2">
            <details v-for="item in 3" :key="item" class="mb-4">
              <summary class="font-semibold bg-gray-200 rounded-md py-2 px-4">
                What do our customers say about us?
              </summary>

              <span>
                In the end it’s all about the customers opinion. We are very pleased with
                the good appreciation of our customers. Our service is valued on average
                with an 8,5/10 based on 5797 rating. We are proud of the high rating we
                have received.
              </span>
            </details>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
