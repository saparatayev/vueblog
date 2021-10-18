<template>
  <div>
    <Navbar />
    <router-view/>
    <footer>
      Footer
    </footer>
  </div>
</template>

<script>
import Navbar from '@/components/layouts/Navbar.vue'

export default {
  components: {
    Navbar
  }  
}
</script>
