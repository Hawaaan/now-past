<!-- src/components/Navbar.vue -->
<template>
  <nav class="bg-blue-600 text-white p-4 flex justify-between items-center">
    <h1 class="text-xl font-bold">MyApp</h1>
    <ul class="flex space-x-4">
      <li><a href="#" class="hover:text-gray-300">Home</a></li>
      <li><a href="#" class="hover:text-gray-300">About</a></li>
      <li><a href="#" class="hover:text-gray-300">Contact</a></li>
    </ul>
  </nav>
</template>

<script>                
export default {
  name: 'Navbar',
}
</script>
