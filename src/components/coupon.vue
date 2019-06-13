<!--<template>-->
<!--    -->
<!--</template>-->

<script>
    export default {
        name: "coupon",

        template: "<input placeholder='Enter your Free Ride Code' @blur='onCouponApplied'>",

        methods: {
            onCouponApplied(){
                this.$emit('applied');
            }
        }
    }

</script>

<!--<style scoped>-->

<!--</style>-->
