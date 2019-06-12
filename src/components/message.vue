<!--<template>-->
<!--    -->
<!--</template>-->

<script>
    export default {
        // name: "message",
        props: ['title', 'body'],
        template: '<article>' +
            '<div class="message-header">' +
            '{{title}}' +
            '</div>' +
            '<div class="message-body">' +
            '{{body}}' +
            '</div>' +
            '</article>'

    }
</script>

<!--<style scoped>-->

<!--</style>-->
