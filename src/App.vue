<template>
  <div>
    <Navbar />
    <Sidebar/>
  <login/>
  <signUp/>
    <main class="">
    </main>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Sidebar from './components/Sidebar.vue'
import login from './components/login.vue'
import signUp from './components/signUp.vue'

export default {
  components: {
    Navbar,
    Sidebar,
    login,
    signUp  
  }
}
</script>
