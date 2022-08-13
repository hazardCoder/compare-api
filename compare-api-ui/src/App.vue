<template>
    <div height=window.outerHeight>
      <el-row :gutter="20" justify="center" type="flex">
        <el-col :span="8">
          <div class="grid-content bg-purple">
            <p>设计API</p>
            <DesignApi></DesignApi>
          </div>
        </el-col>
        <el-col :span="8">
          <div class="grid-content bg-purple">
            <p>全量API</p>
            <AllApi></AllApi>
          </div>
        </el-col>
        <el-col :span="8">
          <div class="grid-content bg-purple">
            <p>注册API</p>
            <RegistedApi></RegistedApi>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="20" justify="center" type="flex" align="bottom">
        <el-col :span="24">
          <div class="grid-content bg-purple">
            <DiffApi></DiffApi>
          </div>
        </el-col>
      </el-row>
    </div>
</template>

<script>
import DesignApi from './components/DesignApi.vue'
import AllApi from './components/AllApi.vue'
import RegistedApi from './components/RegistedApi.vue'
import DiffApi from './components/DiffApi.vue'

export default {
  name: 'design',
  components: {
    DesignApi,
    AllApi,
    RegistedApi,
    DiffApi
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
  .el-col {
    border-radius: 4px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
</style>
