<template>
  
  <div>
    <Nav />
    <counter />
    <div class="main-container flex">
    <LeftSidebar /> 
    <MainContent />
    </div>
    
    <Footer />

  </div>

</template>

<script>
import Nav from './components/Nav'
import Counter from './components/Counter'
import LeftSidebar from './components/LeftSidebar'
import MainContent from './components/MainContent'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Nav,
    Counter,
    LeftSidebar,
    MainContent,
    Footer
  }
}
</script>
