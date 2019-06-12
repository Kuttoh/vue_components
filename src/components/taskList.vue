<!--<template>-->
<!--    -->
<!--</template>-->

<script>
    import newTask from "./newTask"
    export default {
        components: {newTask},

        template: "<div><newTask v-for='(item, index) in items' v-bind:key='item.id' v-if='item.complete'>{{item.description}}</newTask></div>",
        data(){
            return{
                items: [
                    {description: "Wake-up", complete: true},
                    {description: "Spread your bed", complete: true},
                    {description: "Shower", complete: true},
                    {description: "Eat breakfast", complete: false},
                    {description: "Go to work", complete: true}
                ]
            }
        }
    }
</script>

<!--<style scoped>-->

<!--</style>-->
