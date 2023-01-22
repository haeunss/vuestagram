<template>
  <div>
    <InstaPost :PostData="PostData[i]" v-for="(post,i) in PostData" :key="i"/>
    <!-- <InstaPost :PostData="PostData[1]"/>
    <InstaPost :PostData="PostData[2]"/> -->
    <!-- <InstaPost/>
    <InstaPost/> -->
  </div>
</template>

<script>
import InstaPost from './InstaPost.vue'

export default {
  name: 'InstaContainer',
  components: {
    InstaPost: InstaPost,
  },
  props:{
    PostData:Array,
  }
}
</script>

<style>

</style>