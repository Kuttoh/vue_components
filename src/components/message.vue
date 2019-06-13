<!--<template>-->
<!--    -->
<!--</template>-->

<script>
    export default {
        // name: "message",
        props: ['title', 'body'],

        template: '<article v-show="isVisible">' +
            '<div class="message-header">' +
            '{{title}}' +
            '<button type="button" @click="isVisible = false">x</button>' +
            '</div>' +
            '<div class="message-body">' +
            '{{body}}' +
            '</div>' +
            '</article>',

        data(){
            return{
                isVisible: true
            }
        }

        // methods: {
        //     hideModal(){
        //         this.isVisible = false
        //     }
        // }

    }
</script>

<!--<style scoped>-->

<!--</style>-->
