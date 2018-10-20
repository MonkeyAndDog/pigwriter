<template>
  <el-row type="flex" justify="center" >
    <el-col :xs="24" :sm="24" :md="14" :lg="13">
      <el-container id="app">
        <el-header>
          <PageHeader></PageHeader>
        </el-header>
        <el-main>
          <router-view/>
        </el-main>
      </el-container>
    </el-col>
  </el-row>
</template>

<script>
  import PageHeader from "@/components/PageHeader";

  export default {
    name: 'App',
    components: {PageHeader}
  }
</script>

<style>
</style>
