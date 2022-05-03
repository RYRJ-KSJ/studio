<template>
  <div class="att-wrapper" ref="attWrapper">
    <div class="attContainer">
      <div class="content">
        <img src="../assets/noattent.png" alt="">
      </div>
      <div class="title">Others following</div>
      <div class="attent-list">
        <ul>
          <li v-for="(a,index) in attentList" class="attent-item">
            <div class="left">
              <img :src="a.img" alt="">
            </div>
            <div class="right">
              <div class="a-title">
                <h3>{{a.name}}</h3>
                <span>{{a.desc}}</span>
              </div>
              <div class="a-btn">
                <button>Follow</button>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import BScroll from 'better-scroll'
export default {
  data () {
    return {
      attentList: [
        {
          img: 'static/img/a1.png',
          name: 'xyz_999',
          desc: 'Daily routine'
        },
        {
          img: 'static/img/a2.png',
          name: 'xyz_888',
          desc: 'Dresses lover'
        },
        {
          img: 'static/img/a3.png',
          name: 'xyz_777',
          desc: 'P style'
        },
        {
          img: 'static/img/a4.png',
          name: 'xyz_666',
          desc: 'gen z'
        },
      ]
    }
  },
  methods: {
    _initScroll () {
      this.attentScroll = new BScroll(this.$refs.attWrapper, {
        click: true,
        scrollY: true
      });
    }
  },
  created () {
    this.$nextTick( () => {
      this._initScroll()
    })
  }
}
</script>
<style lang="stylus" rel="stylesheet/stylus">
.att-wrapper
  width 100%
  top 2.62rem
  bottom 0
  position absolute
  overflow hidden
  .attContainer
    width 100%
    // min-height 200%
    .content
      width 100%
      img 
        width 100%
    .title
      width 100%
      height 1.11rem
      line-height 1.11rem
      font-size 0.46rem
      color #9c9d9e
      margin-left 0.39rem
      background-color #f5f8fa
    .attent-list
      width 100%
      ul > li
        list-style none 
      .attent-item
        padding 15px
        display flex
        flex-direction row
        background #fff
        .left
          margin-right 10px
          img 
            width 50px
            height 50px
        .right
          flex 1
          display flex
          flex-direction row
          justify-content space-between
          .a-title
            font-size 16px
          .a-btn
            width 70px
            height 30px
            margin-top 12px
            button
              width 100%
              height 100%
              color #ff2741
              border none
              border-radius 4px
              background #fff
              outline none
              border 1px solid #ff2741
</style>

