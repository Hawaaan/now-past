<!-- LoginForm.vue -->
<template>
  <form class="max-w-sm p-4 bg-white rounded shadow space-y-4 absolute top-[350px] left-[270px]">
    <h2 class="text-xl font-semibold text-center">Sign Up</h2>
    <input type="email" placeholder="Email"
      class="w-full border px-4 py-2 rounded focus:outline-none focus:ring" />
    <input type="password" placeholder="Enter new Password"
      class="w-full border px-4 py-2 rounded focus:outline-none focus:ring" />
    <button type="submit"
      class="w-full bg-blue-600 text-white py-2 rounded hover:bg-blue-700">
      Sign Up
    </button>
  </form>
</template>
<script>
export default {
  name: 'signUp',
}
</script>