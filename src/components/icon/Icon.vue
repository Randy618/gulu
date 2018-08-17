<template>
    <i :class="classes"></i>
</template>

<script>
    const prefixCls="fa";

    export default {
        name: "Icon",
        props:{
            type:{
                type:String,
                default:''
            }
        },
        computed:{
            classes(){
                return [
                    {
                        [`${prefixCls}`]: this.type !== ''&&this.type.search(prefixCls)!=-1,
                        [`${this.type}`]: this.type !== ''
                    }
                ]
            }
        }
    }
</script>