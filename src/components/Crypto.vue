<template>
 <div class="crypto">
    <div id="crypto-container" v-for="(value, key) in cryptos" :key="value.id">
        <span class="right">{{ key }}</span>
        <span class="right">{{ value.name }}</span>
        <span class="left">{{ value.symbol }}</span>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

export default {
    name: 'Crypto',
    data: () => ({
        cryptos: [],
        errors: []
    }),
    created () {
    axios.get('https://api.coingecko.com/api/v3/coins/list?include_platform=false')
      .then(response => {
        this.cryptos = response.data
        console.log(response)         // This will give you access to the full object
      })
      .catch(e => {
        this.errors.push(e)
      })
  }
}
</script>

<style>
</style>