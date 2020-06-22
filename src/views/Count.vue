<template>
  <div class="about">
    <h1>This is an Count page</h1>
    <p>{{ count }}</p>
    <button @click='increment()'>+</button>
    <button @click='decrement()'>-</button>
  </div>
</template>
<script>
export default {
    data(){
        return{

        }    
    },
    methods: {
        increment () {
            this.$store.commit('increment')
        },
        decrement () {
            this.$store.commit('decrement')
        }
    },
        computed: {
        count () {
            return this.$store.getters.count;
        }
    },
}
</script>>