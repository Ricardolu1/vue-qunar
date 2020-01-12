<template>
  <div>
    <div class="title">周末去哪</div>
    <ul>
      <li class="item border-bottom" v-for="item of weekendList" :key="item.id">
        <div class="item-img-wrapper">
          <img :src="item.imgUrl" alt="" class="item-img">
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name:'HomeWeekend',
  components: {

  },
  data () {
    return {
      weekendList:[
        {
          id:'0001',
          imgUrl:'http://img1.qunarzz.com/sight/source/1812/b4/e9d7f043c4fadf.jpg_r_640x214_713df0cf.jpg',
          title:'大连圣亚海洋世界',
          desc:'浪漫大连首站，浪漫的海洋主题公园'
        },
        {
          id:'0002',
          imgUrl:'http://img1.qunarzz.com/sight/source/1812/b4/e9d7f043c4fadf.jpg_r_640x214_713df0cf.jpg',
          title:'大连圣亚海洋世界',
          desc:'浪漫大连首站，浪漫的海洋主题公园'
        },
        {
          id:'0003',
          imgUrl:'http://img1.qunarzz.com/sight/source/1812/b4/e9d7f043c4fadf.jpg_r_640x214_713df0cf.jpg',
          title:'大连圣亚海洋世界',
          desc:'浪漫大连首站，浪漫的海洋主题公园'
        },
      ]
    }
  },
  methods: {

  },
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl';
  .title
    line-height .8rem
    background #eee
    text-indent .2rem
  .item-img-wrapper
    height 37.8vw
    .item-img
      width 100%
  .item-info
    padding  .14rem .2rem .2rem .2rem 
    .item-title
      ellipsis()
      line-height .54rem
      font-size .32rem
    .item-desc
      ellipsis()
      line-height .4rem
      color #ccc


</style>