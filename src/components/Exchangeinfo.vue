<script setup lang="ts">
const priceTicker = [
  {
    symbol: "BNBBUSD",
    price: "319.10000000",
  },
  {
    symbol: "BTCBUSD",
    price: "31626.02000000",
  },
  {
    symbol: "ETHBUSD",
    price: "1972.19000000",
  },
  {
    symbol: "LTCBUSD",
    price: "68.80000000",
  },
  {
    symbol: "TRXBUSD",
    price: "0.08077000",
  },
  {
    symbol: "XRPBUSD",
    price: "0.41750000",
  },
  {
    symbol: "BNBUSDT",
    price: "319.30000000",
  },
  {
    symbol: "BTCUSDT",
    price: "31649.39000000",
  },
  {
    symbol: "ETHUSDT",
    price: "1973.46000000",
  },
  {
    symbol: "LTCUSDT",
    price: "68.80000000",
  },
  {
    symbol: "TRXUSDT",
    price: "0.08082000",
  },
  {
    symbol: "XRPUSDT",
    price: "0.41770000",
  },
  {
    symbol: "BNBBTC",
    price: "0.01008700",
  },
  {
    symbol: "ETHBTC",
    price: "0.06235000",
  },
  {
    symbol: "LTCBTC",
    price: "0.00217500",
  },
  {
    symbol: "TRXBTC",
    price: "0.00000256",
  },
  {
    symbol: "XRPBTC",
    price: "0.00001320",
  },
  {
    symbol: "LTCBNB",
    price: "0.21660000",
  },
  {
    symbol: "TRXBNB",
    price: "0.00025320",
  },
  {
    symbol: "XRPBNB",
    price: "0.00130800",
  },
];
</script>

<template>
  <div class="container mx-auto my-8">
    <div class="table w-full border border-4 border-blue-500">
      <div class="table-caption">Symbol Price Ticker</div>
      <div class="table-header-group">
        <div class="table-row">
          <div class="table-cell">Pair</div>
          <div class="table-cell">Price</div>
        </div>
      </div>
      <div
        class="table-row-group"
        v-for="item in priceTicker"
        :key="item.symbol"
      >
        <div class="table-row">
          <div class="table-cell">{{ item.symbol }}</div>
          <div class="table-cell">{{ item.price }}</div>
        </div>
      </div>
      <div class="table-footer-group">
        <div class="table-row">
          <div class="table-cell">Totals</div>
          <div class="table-cell">21,000</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.table-cell {
  @apply py-2 px-4 border border-blue-500 text-center;
}
</style>
