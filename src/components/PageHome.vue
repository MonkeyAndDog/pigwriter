<template>
  <el-row>
    <el-col>

      <el-card class="content-card" shadow="hover">
        <div slot="header" class="clearfix">
          <span>卡片名称</span>
          <el-button style="float: right; padding: 3px 0" type="text">操作按钮</el-button>
        </div>
        <div v-for="o in 4" :key="o" style="overflow-wrap: break-word">
          {{'列表内容 ' + o }}
        </div>
      </el-card>
      <el-card class="content-card" shadow="hover">
        <div slot="header" class="clearfix">
          <span>卡片名称</span>
          <el-button style="float: right; padding: 3px 0" type="text">操作按钮</el-button>
        </div>
        <div v-for="o in 4" :key="o" style="overflow-wrap: break-word">
          {{'列表内容 ' + o }}
        </div>
      </el-card>
      <el-card class="content-card" shadow="hover">
        <div slot="header" class="clearfix">
          <span>卡片名称</span>
          <el-button style="float: right; padding: 3px 0" type="text">操作按钮</el-button>
        </div>
        <div v-for="o in 4" :key="o" style="overflow-wrap: break-word">
          {{'列表内容 ' + o }}
        </div>
      </el-card>
    </el-col>
  </el-row>
</template>

<script>
  export default {
    name: "PageShowArticles"
  }
</script>

<style scoped>
  .content-card {
    margin-bottom: 12px;
  }
</style>
