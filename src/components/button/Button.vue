<template>
    <button type="button" :class="classes"><slot></slot></button>
</template>

<script>
    import { oneOf } from '../../utils/assist';

    const prefixCls = 'btn';

    export default {
        name: "MButton",
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
                default:'',
                validator (value) {
                    return oneOf(value, ['sm','lg', 'hg','']);
                }
            }
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
                        [`${prefixCls}-${this.size}`]: this.size!=='',
                    }
                ];
            }
        }
    }
</script>
