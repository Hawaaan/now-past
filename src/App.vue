<template>
  <div>
    <Navbar />
    <Sidebar/>
  <login/>
    <main class="">
    </main>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Sidebar from './components/Sidebar.vue'
import login from './components/login.vue'

export default {
  components: {
    Navbar,
    Sidebar,
    login
  }
}
</script>
