<template>
    <div class="hello">
        <h2>Profile Page({{user_id}})</h2>
    
    </div>
</template>

<script>
export default {
    name: 'Profile',
    data () {
        return {
            user_id: this.$route.params.user_id
        }
    },
    methods: {
        updateId(){
            this.user_id = this.$route.params.user_id
        }
    },
    watch:{
        $route: 'updateId'
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h2{
        color: green;
    }
</style>
