<template>
    <div>
        <h1>The User Page</h1>
        <hr>
        <!-- <p>Loaded ID: {{ $route.params.id }}</p> -->
        <button class="btn btn-primary" @click="navigateToHome">Go to Home</button>
        <router-view></router-view>
    </div>

</template>

<script>
    export default {
        // data() {
        //     return {
                
        //     }
        // },
        // watch: {
        //     '$route'(to, from) {
        //         this.id = to.params.id;
        //     }
        // },
        methods: {
            navigateToHome() {
                this.$router.push({ name: 'home' });
            }
        }
    }
</script>
