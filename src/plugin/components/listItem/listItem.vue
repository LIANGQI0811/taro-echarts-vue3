<template>
  <view>
    <view>name: {{name}}</view>
    <view>value: {{value}}</view>
  </view>
</template>

<script>
import { ref } from 'vue'
import './listItem.scss'
export default {
  props: ['name', 'value']
}
</script>
