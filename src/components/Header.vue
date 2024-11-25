<script setup>

</script>

<template>
    <div class="bg-white py-12 px-6 text-center">
      <!-- Blog Title -->
      <p class="text-purple-600 font-medium mb-2">Our blog</p>
      <h1 class="text-3xl font-extrabold text-gray-900 mb-4">Stories and interviews</h1>
      <p class="text-gray-600 mb-6">
        Subscribe to learn about new product features, the latest in technology,
        solutions, and updates.
      </p>
  
      <!-- Subscription Form -->
      <div class="flex flex-col gap-4 md:flex-row justify-center items-center space-x-2 w-full">
        <!-- Email Input -->
        <input
          type="email"
          placeholder="Enter your email"
          class="w-full max-w-md border border-gray-300 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-purple-500"
        />
        <!-- Subscribe Button -->
        <button
          class="sm:w-full  md:w-auto bg-purple-600 text-white font-medium px-6 py-2 rounded-lg hover:bg-purple-700 focus:outline-none focus:ring-2 focus:ring-purple-500"
        >
          Subscribe
        </button>
      </div>
  
      <!-- Privacy Policy -->
      <p class="text-gray-500 mt-4 text-sm">
        We care about your data in our
        <a href="#" class="text-purple-600 underline hover:text-purple-800">
          privacy policy
        </a>
      </p>
    </div>
  </template>
  
  
  