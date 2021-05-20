<template>
  <div class="home">
    <a href="../../static/download/111.txt" download="test">测试下载</a>
    <el-button type="success" class="to_lead" @click.native="exportData()">
      <span class="glyphicon glyphicon-arrow-up"></span> 导出
    </el-button>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" />使用公共组件 -->
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";//导入公共组件

export default {
  name: "Home",
  components: {
    // HelloWorld//注册公共组件
  },
  data() {},
  methods: {
    exportData() {
      location.href = "../../static/download/111.txt";
    }
  }
};
</script>
