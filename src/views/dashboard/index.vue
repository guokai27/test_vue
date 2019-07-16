<template>
  <div class="dashboard-container">
    <el-row :gutter="18">
      <el-col :span="8">
        <el-card shadow="never">
          <h3>点击图片进入城域网大屏</h3>
          <a :href='"#/dash"' style="color: #12a7ff">
            <img src="../../assets/DG.png">
          </a>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>
<script>
  export default {
    name: 'dashboard',
    mounted() {
      if (this.$root.ORDERID) {
        this.$root.ORDERID = false
        this.$router.go(0)
      }
    },
    data() {
      return {}
    },
  }
</script>
