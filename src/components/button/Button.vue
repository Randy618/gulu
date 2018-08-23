<template>
    <button type="button" :class="classes" :data-style="loadings">
        <i :class="icons" v-if="icons"></i>
        <slot></slot>
    </button>
</template>

<script>
    import { oneOf } from '../../utils/assist';

    const prefixCls = 'btn';
    const prefixIcon = 'fa';

    export default {
        name: "Button",
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
            active:{
                type:Boolean,
                default:false
            },
            iconRounded:{
                type:Boolean,
                default:false
            },
            block:{
                type:Boolean,
                default:false
            },
            icon:String,
            pull:{
                type:String,
                validator(value){
                    return oneOf(value,["left","right"])
                }
            },
            loading:{
                type:String,
                validator(value){
                    return oneOf(value,['expand-left','expand-right','zoom-in'])
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
                        [`${prefixCls}-icon`]: this.iconRounded,
                        [`${prefixCls}-block`]: this.block,
                        [`ladda-button`]: this.loading!=='',
                        [`active`]: this.active,
                    }
                ];
            },
            icons(){
                return [
                    {
                        [`${prefixIcon}`]: this.icon !== ''/*&&this.icon.isPrototypeOf(${prefixCls})*/,
                        [`${this.icon}`]: this.icon !== '',
                        [`pull-${this.pull}`]: this.pull!==undefined&&this.pull!=='',
                    }
                ]
            },
            loadings(){
                return [{ [`${this.loading}`]: this.loading!==undefined&&this.loading!==''}]
            }

        }
    }
</script>
