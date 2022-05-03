<template>
    <div class="panel">
        <div class="header">
            <img src="../assets/wm.png" alt="watermelon">
            <div>Username {{user.name}}</div>
        </div>
        <div class="content">
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon1.png" alt="look">
                </div>
                <div class="text">
                    <span>Following</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon2.png" alt="">
                </div>
                <div class="text">
                    <span>Likes</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon3.png" alt="">
                </div>
                <div class="text">
                    <span>Message</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon4.png" alt="">
                </div>
                <div class="text">
                    <span>Shopping cart</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon5.png" alt="">
                </div>
                <div class="text">
                    <span>Orders</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon6.png" alt="">
                </div>
                <div class="text">
                    <span>Promotions</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon7.png" alt="">
                </div>
                <div class="text">
                    <span>Lists</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon8.png" alt="">
                </div>
                <div class="text">
                    <span>VIP</span>
                </div>
            </div>
            <div class="con_item">
                <div class="img">
                    <img src="../assets/icon9.png" alt="">
                </div>
                <div class="text">
                    <span>Settings</span>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            user: []
        }
    }
}
</script>
<style lang="stylus" rel="stylesheet/stylus" scoped>
.panel
    width 100%
    height 100%
    background white
    .header
        width 100%
        height 10%
        font-size 20px
        margin-top 60px
        text-align center
        img 
            width 40px
            height 40px
    .content
        width 80%
        padding 30px
        .con_item
            height 25px
            line-height 25px
            font-size 16px
            margin-bottom 30px
            display flex
            flex-direction row
            .img 
                margin-right 15px
                img
                    width 25px
                    height 25px
            .text 
                height 25px
                line-height 25px
</style>

