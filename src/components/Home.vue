<template>
  <div>
    <span>这是Home组件</span>
    <el-button type="info" @click="logout">退出</el-button>
    <span>Admin</span>
  </div>
</template>

<script>
export default {
  methods: {
    logout() {
      window.sessionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style>
</style>