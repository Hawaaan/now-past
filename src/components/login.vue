<!-- LoginForm.vue -->
<template>
  <form class="max-w-sm mx-auto p-4 bg-white rounded shadow space-y-4 absolute top-0 left-0 right-0  ml-[19rem] mt-[15rem]">                                                                                               ]">
    <h2 class="text-xl font-semibold text-center">Login</h2>
    <input type="email" placeholder="Email"
      class="w-full border px-4 py-2 rounded focus:outline-none focus:ring" />
    <input type="password" placeholder="Password"
      class="w-full border px-4 py-2 rounded focus:outline-none focus:ring" />
    <button type="submit"
      class="w-full bg-blue-600 text-white py-2 rounded hover:bg-blue-700">
      Login
    </button>
  </form>
</template>
<script>
export default {
  name: 'login',
}
</script>