<template>
  <router-link :to="to">{{ label }}</router-link>
</template>

<script>
export default {
    props: {
        to: {
            type: String,
            required: true
        },
        label: {
            type: String,
            required: true
        }
    }
}
</script>

<style>

</style>