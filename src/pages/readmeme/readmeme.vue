<template>
  <div>
    <view>Vant Weapp组件库官方示例改写到Mpvue框架下</view>
    <mybr/>
    <mybr/>
    <view>https://github.com/aierong/vantweappmpvuedemo</view>
    <mybr/>
    <mybr/>
    <button open-type="share">分享我吧</button>
  </div>
</template>

<script>

  import mybr from '@/components/mybr/mybr.vue'

  export default {
    name : "readmeme" ,
    components : {
      mybr
    } ,
    onShareAppMessage () {
      return {
        title : 'Vant Weapp在mpvue中使用demo' ,
        path : '/pages/index/main' ,
        imageUrl : '/static/img/logo.png'
      }
    } ,
    data () {
      return {}
    } ,

  }
</script>

<style scoped
       src="./readmeme.css">
</style>
