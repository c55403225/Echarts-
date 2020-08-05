<template>
  <div class="common-card">
    <common-card 
      title='累计销售额'
      value='￥5,544,465,4'
    >
    <template>
     <div class="compare-werp">
        <div class="compare">
        <span>日同比</span>
        <span class='emphasis'>7.33%</span>
        <div class="buttom-angle"></div>
      </div>
       <div class="compare">
        <span>月同比</span>
        <span class='emphasis'>38.79%</span>
        <div class="top-angle"></div>
      </div>
     </div>
    </template>
    <template
    v-slot:footer
    >
        <span>昨日销售额 </span>
      <span class='emphasis'>￥54,456,156,15</span>
    </template>
    </common-card>
  </div>
</template>

<script>
import commonCardMixins from './../mixins/commonCardMixins'
export default {
 mixins:[commonCardMixins]
};
</script>

<style lang='scss'>


.compare-werp{
      height: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
    .compare{
      display: flex;
      align-items: center;
      font-size: 12px;
      margin-top: 3px;
      color: #666;
      background: yellow;
 
}

}

</style>
