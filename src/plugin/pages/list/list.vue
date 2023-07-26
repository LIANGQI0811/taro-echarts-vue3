<template>
  <view>
    <list-item
      v-for="item in list"
      :key="item.name"
      :name="item.name"
      :value="item.value" />
  </view>
</template>

<script>
import { ref } from 'vue'
import './list.scss'
import ListItem from '../../components/listItem/listItem.vue'
export default {
  components: {
    'list-item': ListItem
  },
  setup () {
    const list = ref([{
      name: 'A',
      value: '1'
    }, {
      name: 'B',
      value: '2'
    }, {
      name: 'C',
      value: '3'
    }])
    return {
      list
    }
  }
}
</script>
