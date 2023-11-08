<template>
  <div class="parent">
    <p class="title">{{ props.title || '标题' }}</p>
    <slot v-bind="mocks"></slot>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const props = defineProps<{
  title?: string
}>()

const mocks = ref({
  name: 'tom',
  age: 18,
  sex: '男',
  address: '北京市朝阳区',
  phone: '18888888888',
  email: 'hzdkv@example.com',
  qq: '123456789',
  wechat: '123456789',
  weibo: '123456789',
  weixin: '123456789',
  qqzone: '123456789',
  github: '123456789',
  linkedin: '123456789',
  dribbble: '123456789',
  instagram: '123456789',
  medium: '123456789',
  telegram: '123456789',
  twitter: '123456789'
})
</script>

<style scoped lang="less">
.parent {
  width: 100%;
  height: 100%;

  .title {
    font-size: 20px;
    font-weight: 600;
    margin-bottom: 10px;
  }
}
</style>
