<template>
  <h3>Balance: {{ balance }}</h3>
  <h4>Account: {{ account }}</h4>
  <h4>Status: {{ status ? 'Active' : 'Disabled' }}</h4>
  <div v-for="(service, index) in services" :key="index">
    {{index}} - {{ service }}
  </div>
  <hr>
  <BalanceAction 
    text="Increase Balance"
    @action="increase"
  /> <hr>
  <BalanceAction 
    text="Decrease Balance" 
    @action="decrease"
    :disabled="disabled"
  />
</template>

<script>
import BalanceAction from './BalanceAction.vue'

export default {
  components: {
    BalanceAction
  },
  data() {
    return {
      balance: 1000,
      account: 'Savings',
      status: true,
      services: ['deposits','withdrawals','transfers'],
      disabled: false
    }
  },
  methods: {
    increase() {
      this.balance += 100
      this.disabled = false
    },
    decrease() {
      if (this.balance <= 0) {
        this.disabled = true
        alert('Depleted Balance')
        return
      }
      this.balance -= 100
    }
  }
}
</script>

<style>

</style>