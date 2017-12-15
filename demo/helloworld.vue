<template>
    <div>
        <div class="vux-demo">
            <h1></h1>
        </div>
    </div>
</template>

<script>
    let storage = require("../js/util/storageUtil.js");
    export default {
        components: {
        },
        data() {
            return {

            }
        },
        mounted(){
            this.init();
        },
        methods: {
            init() {
                storage.setLocalStorage("name","1");
                console.log(storage.getLocalStorage("name"));
            }
        }
    }
</script>

<style>
    .vux-demo {
        text-align: center;
    }

    .logo {
        width: 100px;
        height: 100px
    }
</style>
