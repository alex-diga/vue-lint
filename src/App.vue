<script setup lang="ts">
import UploadHugeFile from './components/uploadHugeFile.vue'
import MockSlot from './components/mockSlot.vue'
</script>

<template>
  <UploadHugeFile />
  <MockSlot title="测试 slot 插槽传值">
    <template v-slot="mock">
      <div class="mock">
        <div class="slot">{{ mock.name }}</div>
        <div class="slot">{{ mock.address }}</div>
        <div class="slot">{{ mock.age }}</div>
        <div class="slot">{{ mock.dribbble }}</div>
        <div class="slot">{{ mock.email }}</div>
        <div class="slot">{{ mock.medium }}</div>
      </div>
    </template>
  </MockSlot>
</template>

<style scoped lang="less">
.mock {
  width: 100%;
  height: 100%;

  .slot {
    font-size: 14px;
    color: coral;
  }
}
</style>
