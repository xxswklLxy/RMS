<template>
<div id="home">
   <el-button @click="exit" type="success">退出</el-button>
</div>
</template>

<script>
export default {
  name: 'home',
  methods: {
    exit () {
      window.sessionStorage.clear()
      this.$router.push('/login')
      this.$message({
        message: '退出成功',
        type: 'success'
      })
    }
  }
}
</script>

<style>

</style>
