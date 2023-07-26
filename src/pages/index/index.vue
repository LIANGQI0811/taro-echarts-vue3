<template>
  <view class="index">
    <text>{{msg}}</text>
    <avatar />
    <navigator url='plugin://myPlugin/list'>
      Go to pages/list!
    </navigator>
  </view>
</template>

<script>
import { ref } from 'vue'
import './index.scss'

export default {
  setup () {
    const msg = ref('Hello world')
    return {
      msg
    }
  }
}
</script>
