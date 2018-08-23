<template>
    <div :class="classes">
        <slot></slot>
    </div>
</template>

<script>
    const prefixCls = 'btn-group';

    export default {
        name: "MButtonGroup",
        props:{
            vertical:{
                type:Boolean,
                default:false
            }
        },
        computed:{
            classes(){
                return [
                    `${prefixCls}`,
                    {
                        [`${prefixCls}-vertical`]:this.vertical
                    }
                ]
            }
        }
    }
</script>