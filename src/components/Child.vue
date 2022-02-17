<template>
    <div>
    <h1>Child Component</h1>
    <h3>{{name}}</h3>
    <h3 v-for="user in users" :key="user.name">
        {{users.name}}
    </h3>
    

    
    </div>
</template>

<script>
    export default {
        name:"Child",
        props: {
            name,
        },

        
    }
</script>

<style lang="scss" scoped>

</style>