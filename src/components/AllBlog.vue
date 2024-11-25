<script >
import data from '../data2.json'; // Adjust the path to your JSON file

export default {
  data() {
    return {
      items: data, // Assign the imported data to the items array
    };
  },
  methods: {
    // Method to map tag IDs to specific colors
    getHashtagColor(tagId) {
      const colorMapping = {
        Purple: "text-[#6941C6] bg-[#F9F5FF]", // Purple
        Indigo: "text-[#3538CD] bg-[#EEF4FF]", // Blue
        Pink: "text-[#C11574] bg-[#FDF2FA]", // Pink
        Blue: "text-[#026AA2] bg-[#F0F9FF]", // Purple
      };

      return colorMapping[tagId] || "bg-gray-200 text-gray-600"; // Default color if not found
    },
  },
};
</script>
<template>
    
    <div class="container mx-auto mt-6 w-[100vw] md:w-[90vw] flex flex-col justify-center pb-[100px]">
        <h1 class="text-bold p-4">All Blog Posts</h1>
      <!-- Grid Layout -->
      <div class="grid grid-cols-1 gap-6 md:grid-cols-3 md:grid-rows-2">
        <!-- Loop through the items -->
        <div
          v-for="item in items"
          :key="item.id"
          class="bg-white rounded-lg shadow-md p-4"
        >
          <!-- Image -->
          <img
            :src="item.img"
            alt="Card Image"
            class="rounded-lg w-full mb-4"
          />
          <!-- Name and Date -->
          <div class="text-sm mb-2 text-customPurple ">
            <span class="font-medium ">{{ item.name }}</span>
            &bull;
            <span>{{ item.date }}</span>
          </div>
          <!-- Title -->
          <div>
            <h2 class="text-[18px] font-semibold text-gray-900 mb-2 flex items-center justify-between ">
                {{ item.title }}
                <i class="pi pi-arrow-up-right ml-2 text-sm"></i>
                
            </h2>

          </div>
          <!-- Description -->
          <p class="text-gray-700 mb-4 text-[14px] leading-relaxed">{{ item.description }}</p>
          <!-- Hashtags -->
          <div class="flex flex-wrap gap-2">
            <span
              v-for="(hashtag, index) in Object.values(item.hashtags)"
              :key="index"
              
              :class="getHashtagColor(hashtag.id)"
              class=" text-xs font-medium px-2 py-1 rounded border rounded-full"
            >
              {{ hashtag.tag }}
            </span>
          </div>
        </div>
      </div>
    </div>
  </template>
  