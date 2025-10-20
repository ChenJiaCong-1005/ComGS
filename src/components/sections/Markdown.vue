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
.no-hover {
  max-width: 100%;       /* 图片不会超过容器宽度 */
  height: auto;          /* 保持原始比例 */
  display: block;        /* 避免 inline 元素间距 */
  margin: 1rem auto;     /* 居中显示 */
  box-shadow: none !important;
  border: none !important;
  transition: none !important;
  object-fit: contain;
}

.no-hover:hover {
  box-shadow: none !important;
  transform: none !important;
  opacity: 1 !important;
}
</style>
