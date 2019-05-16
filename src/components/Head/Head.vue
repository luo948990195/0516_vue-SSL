<template>
  <div>
    <div class="header">
      <div class="header-nav">
        <p>2</p>
        <p>3</p>
      </div>
    </div>
    <div class="header">
      <div class="header-info">
        <el-tabs v-model="activeName" @tab-click="handleClick">
          <el-tab-pane>
            <span slot="label"><i class="el-icon-notebook-2"></i> 申请证书</span>申请证书
          </el-tab-pane>
          <el-tab-pane>
            <span slot="label"><i class="el-icon-s-management"></i> 证书管理</span>证书管理
          </el-tab-pane>
          <el-tab-pane>
            <span slot="label"><i class="el-icon-date"></i> 账户管理</span>账户管理
          </el-tab-pane>
          <el-tab-pane>
            <span slot="label"><i class="el-icon-s-goods"></i> 财务管理</span>财务管理
          </el-tab-pane>
          <el-tab-pane>
            <span slot="label"><i class="el-icon-s-tools"></i> 系统设置</span>系统设置
          </el-tab-pane>
          <el-tab-pane>
            <span slot="label"><i class="el-icon-s-tools"></i> 系统设置</span>系统设置
          </el-tab-pane>
        </el-tabs>
        <el-button type="success" class="right">邀请用户购买，返现5%</el-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
      return {
        activeName: 'second'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  border: 1px solid #000;
  height: 100px;
  display: flex;
  justify-content:center;
  align-items:center;
  position: relative;
}
.header-nav {
  border: 1px solid #000;
  width: 80%;
  height: 80px;
  display: flex;
  justify-content:space-between;
  align-items:center;
}
.header-info {
  width: 80%;
}
.right {
  position: absolute;
  right: 200px;
  bottom: 45px;
}
.header-info i {
  font-size: 1.2rem;
}
</style>
