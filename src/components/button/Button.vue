<template>
    <button type="button" :class="classes">
        <i :class="icons" v-if="icons"></i>
        <slot></slot>
    </button>
</template>

<script>
    import Icon from '../icon/Icon';
    import { oneOf } from '../../utils/assist';

    const prefixCls = 'btn';
    const prefixIcon = 'fa';

    export default {
        name: "Button",
        components:{Icon},
        props:{
            type:{
                type:String,
                default:'default',
                validator (value) {
                    return oneOf(value, ['white','default', 'primary', 'success', 'info', 'blue', 'warning', 'danger', 'dark']);
                }
            },
            embossed:{
                type:Boolean,
                default:false
            },
            rounded:{
                type:Boolean,
                default:false
            },
            transparent:{
                type:Boolean,
                default:false
            },
            square:{
                type:Boolean,
                default:false
            },
            size:{
                type:String,
                validator (value) {
                    return oneOf(value, ['sm','lg', 'hg']);
                }
            },
            icon:String
        },
        computed: {
            classes () {
                return [
                    `${prefixCls}`,
                    `${prefixCls}-${this.type}`,
                    {
                        [`${prefixCls}-embossed`]: this.embossed,
                        [`${prefixCls}-rounded`]: this.rounded,
                        [ `${prefixCls}-transparent`]: this.transparent,
                        [`${prefixCls}-square`]: this.square,
                        [`${prefixCls}-${this.size}`]: this.size,
                    }
                ];
            },
            icons(){
                return [
                    {
                        [`${prefixIcon}`]: this.icon !== ''&&this.icon.startsWidth(prefixIcon),
                        [`${this.icon}`]: this.icon !== ''
                    }
                ]
            }

        }
    }
</script>
