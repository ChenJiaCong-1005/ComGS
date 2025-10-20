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
  box-shadow: none !important;
  transform: none !important;
  transition: none !important;
  border: none !important;
}

.no-hover:hover {
  box-shadow: none !important;
  transform: none !important;
  opacity: 1 !important;
}
</style>
