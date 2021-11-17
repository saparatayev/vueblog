<template>
  <div>
    <Hero />
    <div>
      <Articles />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Hero from './Hero.vue'
import Articles from '@/components/Articles.vue'

export default {
  name: 'Home',
  components: {
    Hero,
    Articles,
  }
}
</script>
