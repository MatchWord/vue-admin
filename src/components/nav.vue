<template>
    <div>
        <el-menu
            default-active="2"
            class="el-menu-vertical-demo"
            @open="handleOpen"
            @close="handleClose"
            background-color="#545c64"
            text-color="#fff"
            active-text-color="#ffd04b"
            :collapse="isCollapse"
        >
            <el-menu-item index="1">
                <i class="el-icon-menu"></i>
                <span slot="title">导航一</span>
            </el-menu-item>
            <el-menu-item index="2">
                <i class="el-icon-menu"></i>
                <span slot="title">导航二</span>
            </el-menu-item>
            <el-menu-item index="3">
                <i class="el-icon-document"></i>
                <span slot="title">导航三</span>
            </el-menu-item>
            <el-menu-item index="4">
                <i class="el-icon-setting"></i>
                <span slot="title">导航四</span>
            </el-menu-item>
        </el-menu>
    </div>
</template>

<script>
export default {
    data() {
        return {}
    },
    methods: {
        handleOpen() {},
        handleClose() {}
    },
    computed: {
        isCollapse() {
            return this.$store.state.isCollapse
        }
    }
}
</script>

<style scope lang="scss">
.el-menu-vertical-demo {
    height: 100vh;
}
.el-menu-vertical-demo:not(.el-menu--collapse) {
    width: 170px;
    height: 100vh;
}
</style>
