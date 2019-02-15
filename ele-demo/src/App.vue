<template>
  <div id="app">
    222
    <el-button type="primary" @click="get">主要按钮</el-button>
    <el-button type="success">成功按钮</el-button>
    <!-- <el-row>
      <el-col :span="12"><div class="ccc grid-content bg-purple">1</div></el-col>
      <el-col :span="12"><div class="ccc grid-content bg-purple-light">2</div></el-col>
    </el-row> -->
  </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    get(){
      // alert(2)
      axios.get('a.txt').then(function(res){
        console.log(res);
      })
    }
  }
}
</script>

<style lang="less" scoped>
@el-color: red;
  .ccc {
    border: 1px solid @el-color;
  }
</style>

