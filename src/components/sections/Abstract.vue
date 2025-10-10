<script setup>
import abstract from '../mds/abstract.mdx';
</script>

<template>
  <div>
    <el-divider />

    <el-row justify="center">
      <el-col
        class="abstract-wrapper"
        :xs="24"
        :sm="20"
        :md="16"
        :lg="12"
        :xl="12"
      >
        <abstract />
      </el-col>
    </el-row>
  </div>
</template>

<style scoped>
.abstract-wrapper {
  text-align: justify;
}

</style>
