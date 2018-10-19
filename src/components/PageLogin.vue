<template>
  <div class="space">
    <el-row type="flex" justify="center">
      <el-col :xs="24" :sm="24" :md="16" :lg="10">
        <el-input type="text" class="space">
          <template slot="prepend">username</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row type="flex" justify="center">
      <el-col  :xs="24" :sm="24" :md="16" :lg="10">
        <el-input type="text" class="space">
          <template slot="prepend">password</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row type="flex" class="space" justify="center">
      <el-button type="primary" class="space" @click="login">登录<i class="el-icon-upload el-icon--right"></i></el-button>
    </el-row>
  </div>
</template>

<script>
  import store from '../main'
  export default {
    name: "PageLogin",
    methods:{
      login:function () {
        //验证密码，登录系统
        store.store.logged_in = true
      }
    }
  }
</script>

<style scoped>
  .space {
    margin-top: 10px;
  }
</style>
