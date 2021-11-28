<template>
  <div class="container">
    <ColumnList :list="list"></ColumnList>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import 'bootstrap/dist/css/bootstrap.min.css'
import ColumnList, {ColumnProps} from '@/components/ColumnList.vue'
const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'test1专栏',
    description: '这是test1专栏',
    avatar: 'http://www.baidu.com'
  },
  {
    id: 2,
    title: 'test2专栏',
    description: '这是test2专栏',
    avatar: '/assets/logo.png'
  },{
    id: 3,
    title: 'test3专栏',
    description: '这是test3专栏'
    // avatar: 'http://www.baidu.com'
  },{
    id: 4,
    title: 'test4专栏',
    description: '这是test4专栏',
    avatar: 'http://www.baidu.com'
  },{
    id: 5,
    title: 'test5专栏',
    description: '这是test5专栏',
    avatar: 'http://www.baidu.com'
  }
]
  

export default defineComponent({
  name: 'App',
  components: {
    ColumnList
  },
  setup(){
    return {
      list: testData
    }
  }
});
</script>

<style>

</style>
