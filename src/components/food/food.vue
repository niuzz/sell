<template>
    <div v-show="showFlag" class="food">

    </div>

</template>

<script type="text/ecmascript-6">
export default {
    props: {
        food: {
           type: Object
        }
    },
    data () {
        return {
            showFlag: false
        };
    },
    methods: {
        show () {
            this.showFlag = true;
        }
    }
};

</script>

<style lang="stylus" rel="stylesheet/stylus">
    .food {
        position: fixed
        left: 0
        top: 0
        bottom: 48px
        z-index: 30
        width: 100%
        background: #ffffff
        transform: translate3d(0, 0, 0)
        .image-header
            position: relative
            width: 100%
            height: 0
            position-top: 100%
            img
                position: absolute
                top: 0
                left: 0
                width: 100%
                height: 100%

    }

</style>
