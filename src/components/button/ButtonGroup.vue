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
                        [`${prefixCls}-vertical`]:true
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    .btn-group-xs > .btn {
        font-size: 12px;
        line-height: 1.083;
        padding: 6px 9px;
        -webkit-border-radius: 2px;
        -moz-border-radius: 2px;
        border-radius: 2px;
    }
    .btn-group-sm > .btn {
        font-size: 13px;
        line-height: 1.385;
        padding: 9px 13px;
        -webkit-border-radius: 4px;
        -moz-border-radius: 4px;
        border-radius: 4px;
    }
    .btn-group-lg > .btn {
        font-size: 17px;
        line-height: 1.471;
        padding: 10px 19px;
        -webkit-border-radius: 6px;
        -moz-border-radius: 6px;
        border-radius: 6px;
    }
    .btn-group-gh > .btn {
        font-size: 22px;
        line-height: 1.227;
        padding: 13px 20px;
        -webkit-border-radius: 6px;
        -moz-border-radius: 6px;
        border-radius: 6px;
    }
    .btn-group > .btn + .btn {
        margin-left: 0;
    }
    .btn-group > .btn + .dropdown-toggle {
        border-left: 2px solid rgba(52, 73, 94, 0.15);
        padding-left: 12px;
        padding-right: 12px;
    }
    .btn-group > .btn + .dropdown-toggle .caret {
        margin-left: 3px;
        margin-right: 3px;
        margin-top: 0;
    }
    .btn-group > .btn.btn-gh + .dropdown-toggle .caret {
        margin-left: 7px;
        margin-right: 7px;
    }
    .btn-group > .btn.btn-sm + .dropdown-toggle .caret {
        margin-left: 0;
        margin-right: 0;
    }
    .dropdown-toggle .caret {
        margin-left: 8px;
        margin-top: 0;
    }
    .btn-group > .btn {
        font-weight: 400;
    }
    .btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
        border-left: 1px solid rgba(12, 12, 12, 0.1) !important;
    }
    .btn-group > .btn:last-child :not(:first-child) {
        border-left: 1px solid rgba(12, 12, 12, 0.1) !important;
    }
    .btn-group > .dropdown-menu {
        font-weight: 400;
    }
    .btn-group > .popover {
        font-weight: 400;
    }
    .btn-group {
        margin-right: 10px;
    }
    .btn-group:focus .dropdown-toggle {
        -webkit-transition: .25s;
        outline: 0;
        transition: .25s;
    }
    .btn-group i {
        padding-right: 7px;
    }
    .btn-group .btn {
        margin-right: 0;
    }
    .btn-group button.btn-sm {
        height: 25px;
    }
    .btn-group button.btn-xs {
        height: 24px;
    }
    .btn-group button.btn-lg {
        height: 45px;
    }
    .btn-group button.btn-hg {
        height: 52px;
    }
    .btn-group.open .dropdown-toggle {
        -webkit-box-shadow: none;
        box-shadow: none;
        color: rgba(255, 255, 255, 0.75);
    }
    .btn-group.open .dropdown-toggle.btn-default {
        color: #616C76;
    }
    .btn-group > .dropdown-toggle:not(:first-child) {
        border-left: 1px solid rgba(12, 12, 12, 0.1) !important;
    }
    .btn-group-vertical {
        margin-right: 20px;
    }
    .btn-group-vertical .btn {
        margin-bottom: 0;
    }
    .btn-group-vertical .btn i {
        padding-right: 0 !important;
    }
</style>