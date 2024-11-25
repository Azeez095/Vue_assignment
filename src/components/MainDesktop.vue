<script setup>
    import image1 from '/image1.png'
    import image2 from '/image2.png'
    import image3 from '/image3.png'
</script>

<template>
    <div class="flex justify-center">
    <div class="hidden md:grid grid-cols-2 grid-rows-[20vh_20vh] p-4 md:w-[90vw] gap-6">
        <div class="col-start-1 col-end-1 row-start-1 row-end-3 max-h-full" >
            <img
            :src="image1"
            alt="Card Image"
            class="rounded-lg w-full mb-4 object-cover h-[50%]"
          />
          <div>
            <div class="text-sm my-4 text-customPurple">
                <span >Olivia Rhye</span> &bull;<span class="pl-2">20 jan 2022</span>
            </div>
            <div class="flex items-center justify-between">
                <h1 class="font-bold text-2xl mb-4">UX review presentation</h1> 
                <i class="pi pi-arrow-up-right ml-2 text-sm"></i>
            </div>
            <p class="text-gray-700 mb-4 text-[14px] leading-relaxed">How do you create compelling presentations that wow your colleagues and impress your managers?</p>
            <div>
                <span class=" text-xs font-medium px-2 py-1 rounded border rounded-full text-[#6941C6] bg-[#F9F5FF]">Design</span> 
                <span  class=" text-xs font-medium px-2 py-1 rounded border rounded-full mx-3 text-[#3538CD] bg-[#EEF4FF]">Research</span>
                <span  class=" text-xs font-medium px-2 py-1 rounded border rounded-full text-[#C11574] bg-[#FDF2FA]">Presentation</span>
            </div>
          </div>
        </div>
        <div class="col-start-2 col-end-2 row-start-1 row-end-3 flex flex-col justify-between max-h-full">
            <div class="flex justify-between gap-4 align-center w-full">
                <img
                :src="image2"
                alt="Card Image"
                class="rounded-lg w-1/2 h-[80%] object-cover"
                />
                <div>
                    <div class="text-sm text-customPurple">
                        <span >Phoenix Baker</span> &bull;<span class="pl-2">19 jan 2022</span>
                    </div>
                    <div class="flex items-center justify-between">
                        <h1 class="font-bold text-xl mb-4">Migrating to Linear 101</h1> 
                        <i class="pi pi-arrow-up-right ml-2 text-sm"></i>
                    </div>
                    <p class="text-gray-700 mb-4 text-[14px] leading-relaxed">Linear helps streamline software projects, sprints, tasks, and bug tracking. Here’s how to get started.</p>
                    <div>
                        <span class=" text-xs font-medium px-2 py-1 rounded border rounded-full text-[#6941C6] bg-[#F9F5FF]">Design</span> 
                        <span  class=" text-xs font-medium px-2 py-1 rounded border rounded-full mx-3 text-[#3538CD] bg-[#EEF4FF]">Research</span>
                    </div>
                </div>
            </div>

            <div class="flex justify-between gap-4 align-center w-full">
                <img
                :src="image3"
                alt="Card Image"
                class="rounded-lg w-1/2 h-[80%] object-cover"
                />
                <div>
                    <div class="text-sm text-customPurple">
                        <span >Lana Steiner</span> &bull;<span class="pl-2">18 jan 2022</span>
                    </div>
                    <div class="flex items-center justify-between">
                        <h1 class="font-bold text-2xl mb-4">Building your API Stack</h1> 
                        <i class="pi pi-arrow-up-right ml-2 text-sm"></i>
                    </div>
                    <p class="text-gray-700 mb-4 text-[14px] leading-relaxed">The rise of RESTful APIs has been met by a rise in tools for creating, testing, and managing them.</p>
                    <div>
                        <span class=" text-xs font-medium px-2 py-1 rounded border rounded-full text-[#6941C6] bg-[#F9F5FF]">Design</span> 
                        <span  class=" text-xs font-medium px-2 py-1 rounded border rounded-full mx-3 text-[#3538CD] bg-[#EEF4FF]">Research</span>
                    </div>
                </div>
            </div>

            
        </div>
    </div>
</div>
</template>