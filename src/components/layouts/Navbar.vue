<template>
    <nav>
        <div>
            <button class="sm:hidden" v-show="!isVisible" @click="toggle">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
            </button>
            <button class="sm:hidden" v-show="isVisible" @click="toggle">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
            </button>
        </div>
        <div class="flex flex-col sm:flex-row sm:block"
            :class="{'hidden': !isVisible}"    
        >
            <NavbarLink to="/articles" label="Articles" />
            <NavbarLink to="/about" label="About" />
            <NavbarLink to="/contact" label="Contact" />
        </div>
    </nav>
</template>

<script>
import NavbarLink from './NavbarLink.vue'
import { useToggle } from '@/composables/useToggle'

export default {
    components: {
        NavbarLink
    },
    setup() {
        let { isVisible, toggle } = useToggle();

        return {
            isVisible,
            toggle,
        }
    },
}
</script>