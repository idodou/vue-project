<template>
  <div id="app">
    <p class="title">PartyBuy 合约配置</p>
    <div class="contract-box">
      <div class="contract-line">
        <span>
          合约名称
        </span>
        <span>
          部署地址
        </span>
        <span>
          备注
        </span>
      </div>
      <div class="contract-detail" v-for="item in contractList" :key="item.name">
        <span>
          {{item.name}}
        </span>
        <span>
          {{item.address}}
        </span>
        <span>
          {{item.comment}}
        </span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Main',
  data() {
    return {
      contractList: [
        {name:"ParytBuyToken",address:"0xE41B705AFdF605E87188E079B93a1e177b54BB15",comment:"(BNB Smart Chain Testnet)"},
        {name:"ParytBuyToken",address:"0xE41B705AFdF605E87188E079B93a1e177b54BB15",comment:"(BNB Smart Chain)"},
        {name:"PartyBuy",address:"0xb7bA3B2DE78CCAfd4e6b1B1AAd39EfFAE55c06B0",comment:""},
        {name:"测试 USDT",address:"0x2A84A0fA46Bb2F811f7b64f74537224760Ea078B",comment:""},
      ]
    }
  }
}
</script>
<style>
.title{
  font-size: 20px;
}
.contract-box{
  background-color: #cecece;
  padding: 10px 30px;
  color: #393939;
  border-radius: 10px;
}
.contract-line{
  display: flex;
  justify-content: space-between;
  padding-bottom: 10px;
}
.contract-detail{
  display: flex;
  justify-content: space-between;
  color: black;
  font-size: 15px;
  padding-bottom: 6px;
}
</style>