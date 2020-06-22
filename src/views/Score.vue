<template>
  <div class="about">
    <h1>This is an Score page</h1>
    <p>{{ count }}</p>
  </div>
</template>
<script>
export default {
    computed:{
        count () {
            return this.$store.getters.count;
        }
    }
}
</script>>