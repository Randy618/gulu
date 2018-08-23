<template>
    <span :class="classes">
        <slot></slot>
    </span>
</template>

<script>
    import { oneOf } from '../../utils/assist';
    const prefixCls = 'label';

    export default {
        name: "Label",
        props:{
            type:{
                type:String,
                validator(value){
                    return oneOf(value,['default','primary','success','info','warning','danger'])
                }
            },
            badge:{
                type:String,
                validator(value){
                    return oneOf(value,['badge','primary','success','info','warning','danger'])
                }
            }
        },
        computed:{
            classes(){
                return [
                    {
                        [`${prefixCls}`]: this.type!==undefined&&this.type!=='',
                        [`${prefixCls}-${this.type}`]: this.type!==undefined&&this.type!=='',
                        [`badge`]:this.badge!=='',
                        [`badge-${this.badge}`]: this.badge!==''&&this.badge!=="badge"
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>