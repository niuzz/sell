<template>
    <div class="cartcontrol">
        <div class="cart-decrease" v-show="food.count>0">
            <span class="inner icon-remove_circle_outline">
            </span>
        </div>
        <div class="cart-count" v-show="food.count>0">
            {{food.count}}
        </div>
        <div class="cart-add"></div>
    </div>
</template>
<script type="text/ecmascript-6">
    export default {
        props: {
            food: {
                type: Object
            }
        }
    };
</script>

<style lang="stylus" rel="stylesheet/stylus">
    .ccartcontrol
        font-size:0
        .cart-decrease, .cart-add
            display: inline-block
            padding: 6px
            line-height: 24px
            font-size: 24px
            .inner
                display: inline-block
                line-height: 24px
                font-size: 24px
                color: rgb(0, 160, 220)
                transition: all 0.4s linear
                transform: rotate(0)
        .cart-count
            display: inline-block
        .cart-add
            display: inline-block


</style>
