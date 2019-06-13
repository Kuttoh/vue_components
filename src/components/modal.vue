<!--<template>-->
<!--    -->
<!--</template>-->

<script>
    export default {
        name: "modal",

        template:'<div class="modal">\n' +
            '  <div class="modal-background"></div>\n' +
            '  <div class="modal-content">\n' +
            '<p> Lorem ipsum is a placeholder text commonly used to demonstrate the visual form of a document without ' +
            'relying on meaningful content.</p>' +
            '  </div>\n' +
            '  <button class="modal-close is-large" aria-label="close"></button>\n' +
            '</div>',

        data(){
            return{
                showModal: false
            }
        }
    }
</script>

<!--<style scoped>-->

<!--</style>-->
