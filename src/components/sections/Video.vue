<script setup>
</script>

<template>
  <div>
    <el-divider />

    <el-row justify="center">
      <h1 class="section-title">Method Overview</h1>
    </el-row>

    <el-row justify="center">
      <el-col :xs="24" :sm="20" :md="16" :lg="12" :xl="10" >
        
        <!-- 单张图片展示 -->
        <el-container class="image-container">
          <img src="/method_overview.png" alt="Method Overview" class="responsive-img" />
        </el-container>

      </el-col>
    </el-row>
  </div>
</template>

<style scoped>
.image-container {
  margin: 20px 0px 0px 0px;
  text-align: center;
}

.responsive-img {
  width: 100%;
  max-width: 100%;
  height: auto;
  object-fit: contain;
  border-radius: 8px;
  box-shadow: none;
}
</style>
