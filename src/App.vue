<template>
  <Navbar />
  <Login />
  <Crypto />
  <Footer />
</template>

<script>
import Navbar from './components/Navbar'
import Login from './components/Login'
import Footer from './components/Footer'
import Crypto from './components/Crypto'
export default {
  name: 'App',
  components: {
    Navbar,
    Login,
    Footer,
    Crypto
  }
}
</script>

<style>
</style>