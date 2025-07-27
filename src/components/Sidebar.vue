<!-- src/components/Sidebar.vue -->
<template>
  <div class="flex h-screen">
    <!-- Sidebar -->
    <div
      :class="[
        'bg-gray-800 text-white w-64 p-4 space-y-4 transition-transform duration-300 z-20',
        isOpen ? 'translate-x-0' : '-translate-x-full',
        'md:translate-x-0 fixed md:relative top-0 left-0 h-full'
      ]"
    >
      <h2 class="text-2xl font-bold mb-6">dashbord</h2>
      <ul class="space-y-8 ">
        <li class="bg-gray-500 rounded shadow-md shadow-gray-300 text-center p-2 hover:text-gray-300"><a href="#">Sell</a></li>
        <li class="bg-gray-500 rounded shadow-md shadow-gray-300 text-center p-2 hover:text-gray-300"><a href="#">ussers</a></li>
        <li class="bg-gray-500 rounded shadow-md shadow-gray-300 text-center p-2 hover:text-gray-300"><a href="#">supply</a></li>
        <li class="bg-gray-500 rounded shadow-md shadow-gray-300 text-center p-2 hover:text-gray-300"><a href="#">Report</a></li>
         <li class="bg-gray-500 rounded shadow-md shadow-gray-300 text-center p-2 hover:text-gray-300"><a href="#">settings</a></li>
      </ul>
    </div>

    <!-- Overlay (mobile) -->
    <div
      v-if="isOpen"
      class="fixed inset-0 bg-black bg-opacity-50 md:hidden z-10"
      @click="toggleSidebar"
    ></div>

    <!-- Content -->
    <div class="flex-1 p-4 ml-0 md:ml-64 w-full">
      <!-- Top Bar -->
      <div class="md:hidden flex items-center justify-between mb-4">
        <button @click="toggleSidebar" class="text-gray-700">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none"
            viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round"
              stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>

      <!-- Main Content -->
      <div>
        <slot />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggleSidebar() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
