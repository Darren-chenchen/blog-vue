<template>
  <div>
    <tab style="width: 100%;height: 100%" :custom-bar-width="getLineWidth"
         :line-width="2" bar-active-color="rgb(115,109,216)">
      <tab-item :selected="checkedIndex==0" @on-item-click="onItemClick">
        全部笔记
      </tab-item>
      <tab-item :selected="checkedIndex==1" @on-item-click="onItemClick">
        我的作品
      </tab-item>
      <tab-item :selected="checkedIndex==2" @on-item-click="onItemClick">
        我的作品2
      </tab-item>
      <tab-item :selected="checkedIndex==3" @on-item-click="onItemClick">
        我的作品3
      </tab-item>
      <tab-item :selected="checkedIndex==4" @on-item-click="onItemClick">
        我的作品4
      </tab-item>
    </tab>
  </div>
</template>

<script type="text/ecmascript-6">
  import {Tab, TabItem} from 'vux'

  export default {
    components: {
      Tab, TabItem
    },
    data() {
      return {
        checkedIndex: 0
      }
    },
    methods: {
      onItemClick() {},
      getLineWidth() {
          return '60px'
      }
    },
    created() {
    }
  }
</script>

<style lang="scss">
    @import "../../common/scss/base";

</style>
