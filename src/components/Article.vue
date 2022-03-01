<template>
    <div class="grid sm:grid-cols-5 gap-2 sm:gap-12">
        <div class="sm:col-span-3 h-64 sm:h-400px">
            <img src="/images/image-1.jpg" alt="article"
            class="w-full h-full object-cover">
        </div>
        <div class="sm:col-span-2 flex flex-col justify-between">
            <div>
                <div class="text-base text-gray-500">Category name</div>
                <h3 class="mt-1 leading-tight text-2xl">
                    <router-link to="/articles/article-slug"
                    class="hover:text-primary font-bold transition-colors duration-300">Lorem ipsum dolor sit amet consectetur adipisicing elit.</router-link>
                </h3>
                <div class="mt-2 text-gray-700">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia soluta voluptatibus pariatur sed temporibus vitae non necessitatibus, voluptatem magnam exercitationem...</div>
            </div>
            <div class="mt-1 text-base text-gray-500 flex items-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
                <div class="ml-2">
                    5 mins ago
                </div>
            </div>
        </div>
    </div>
</template>