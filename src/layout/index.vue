<template>
  <el-container class="app-layout">
    <Sidebar />
    <el-container>
      <Header />
      <el-main class="app-main">
        <slot />
      </el-main>
    </el-container>
  </el-container>
</template>
<script>
  import Header from './components/Header'
  import Sidebar from './components/Sidebar'
  export default {
    name: 'Layout',
    components: { Header, Sidebar }
  }
</script>
