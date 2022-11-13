<template>
  <section class="bg-white dark:bg-gray-900">
    <div class="container px-6 py-10 mx-auto">
      <div class="mt-8 lg:-mx-6 lg:flex lg:items-center">
        <img
          :key="parking.name"
          class="object-cover w-full lg:mx-6 lg:w-1/2 rounded-xl h-72 lg:h-96"
          src="https://images.unsplash.com/photo-1569154941061-e231b4725ef1?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80"
        />

        <div class="mt-6 lg:w-1/2 lg:mt-0 lg:mx-6">
          <h1
            class="text-3xl font-semibold text-gray-800 capitalize lg:text-4xl dark:text-white"
          >
            {{ parking.name }}
          </h1>

          <p class="mt-3 text-sm text-gray-500 dark:text-gray-300 md:text-sm">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure veritatis sint
            autem nesciunt, laudantium quia tempore delect
          </p>
          <BaseRating :rating="parking.review.stars" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    parking: {
      type: Object,
      default() {
        return {};
      },
    },
  },
};
</script>
