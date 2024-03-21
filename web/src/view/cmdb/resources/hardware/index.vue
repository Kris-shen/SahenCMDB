<script setup>
const tableData = [
  {
    id: "abcdefg123456788",
    name: 'test1',
    status: '使用中',
    serviceProvider: '华为云',
    resource_type: '云服务器',
    specification: 'c7.large.4',
    cpu: '8',
    memory: '32',
    region: '青岛一区',
    AZ: '可用区一',
    createTime:'2023年2月1日',
    privateAddress:'192.168.2.1',
    publicAddress: '133.255.2.100'
  },{
    id: "abcdefg123456789",
    name: 'test1',
    status: '使用中',
    serviceProvider: '华为云',
    resource_type: '云服务器',
    specification: 'c7.large.4',
    cpu: '8',
    memory: '32',
    region: '青岛一区',
    AZ: '可用区一',
    createTime:'2023年2月1日',
    privateAddress:'192.168.2.1',
    publicAddress: '133.255.2.100'
  }]
</script>

<template>
<div>
  <el-card>
    <el-table :data="tableData" style="width: 100%">
      <el-table-column prop="id" label="ID" width="180"/>
      <el-table-column prop="name" label="名称" width="100"/>
      <el-table-column prop="status" label="资源状态" width="80"/>
      <el-table-column prop="serviceProvider" label="服务商" width="80"/>
      <el-table-column prop="resource_type" label="资源类型" width="100"/>
      <el-table-column prop="specification" label="规格"/>
      <el-table-column prop="cpu" label="vCPU" width="80"/>
      <el-table-column prop="memory" label="内存(GB)" width="100"/>
      <el-table-column prop="region" label="区域"/>
      <el-table-column prop="AZ" label="可用区"/>
      <el-table-column prop="createTime" label="资源创建时间"/>
      <el-table-column prop="privateAddress" label="内网地址"/>
      <el-table-column prop="publicAddress" label="公网地址"/>
    </el-table>
  </el-card>
</div>
</template>

<style scoped lang="scss">

</style>