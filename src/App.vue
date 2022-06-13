<template>
  <el-container class="layout-container-demo">
    <el-aside width="200px">
      <el-scrollbar>
        <el-menu :default-openeds="['1', '3']">
          <el-menu-item index="1">
            <template #title>
              <el-icon><House /></el-icon>首页
            </template>
          </el-menu-item>
          <el-menu-item index="2">
            <template #title>
              <el-icon><ChatDotRound /></el-icon>公告
            </template>
          </el-menu-item>
          <el-menu-item index="3">
            <template #title>
              <el-icon><User /></el-icon>教师管理
            </template>
          </el-menu-item>
          <el-menu-item index="4">
            <template #title>
              <el-icon><User /></el-icon>学生管理
            </template>
          </el-menu-item>
          <el-menu-item index="5">
            <template #title>
              <el-icon><Document /></el-icon>图书管理
            </template>
          </el-menu-item>
          <el-menu-item index="6">
            <template #title>
              <el-icon><Monitor /></el-icon>操作历史
            </template>
          </el-menu-item>
          <el-menu-item index="7">
            <template #title>
              <el-icon><User /></el-icon>用户管理
            </template>
          </el-menu-item>
          <el-menu-item index="8">
            <template #title>
              <el-icon><User /></el-icon>角色管理
            </template>
          </el-menu-item>
        </el-menu>
      </el-scrollbar>
    </el-aside>

    <el-container>
      <el-header style="text-align: right; font-size: 12px">
        <div class="toolbar">
          <el-dropdown>
            <el-icon style="margin-right: 8px; margin-top: 1px"
              ><setting
            /></el-icon>
            <template #dropdown>
              <el-dropdown-menu>
                <el-dropdown-item>View</el-dropdown-item>
                <el-dropdown-item>Add</el-dropdown-item>
                <el-dropdown-item>Delete</el-dropdown-item>
              </el-dropdown-menu>
            </template>
          </el-dropdown>
          <span>Tom</span>
        </div>
      </el-header>

      <el-main>
        <el-scrollbar>
          <el-table :data="tableData">
            <el-table-column prop="date" label="Date" width="140" />
            <el-table-column prop="name" label="Name" width="120" />
            <el-table-column prop="address" label="Address" />
          </el-table>
        </el-scrollbar>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
</script>

<style scoped>
.layout-container-demo .el-header {
  position: relative;
  background-color: var(--el-color-primary-light-7);
  color: var(--el-text-color-primary);
}
.layout-container-demo .el-aside {
  color: var(--el-text-color-primary);
  background: var(--el-color-primary-light-8);
}
.layout-container-demo .el-menu {
  border-right: none;
}
.layout-container-demo .el-main {
  padding: 0;
}
.layout-container-demo .toolbar {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  right: 20px;
}
</style>
