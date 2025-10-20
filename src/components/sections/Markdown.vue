<script setup>
import page from '../mds/md.mdx';
</script>

<template>
  <div>
    <el-divider />

    <el-row justify="center">
        <el-col :xs="24" :sm="20" :md="16" :lg="12" :xl="12">
            <page />
        </el-col>
    </el-row>

  </div>
</template>

<style scoped>
/* 禁用 markdown 中插入图片的悬浮效果 */
img {
  max-width: 100%;
  display: block;
  margin: 1rem auto;
  transition: none !important;
  box-shadow: none !important;
  transform: none !important;
  border: none !important;
}

img:hover {
  box-shadow: none !important;
  transform: none !important;
  border: none !important;
  opacity: 1 !important;
}
</style>
