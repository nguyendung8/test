<template>
<div class="signal-page">
  <div class="signal-page-header">
    <Header />
  </div>
  <div class="signal-page-sidebar">
    <Sidebar />
  </div>
  <div class="signal-page-content">
    <Content />
  </div>
  <div class="signal-page-footer">
    <Footer />
  </div>
</div>
</template>

<script>
import Header from '../components/Header.vue';
import Sidebar from '../components/Sidebar.vue';
import Content from '../components/Content.vue';
import Footer from '../components/Footer.vue';
export default {
  name: 'Index',

  components: {
    Header,
    Sidebar,
    Content,
    Footer,
  },
}
</script>
<style>
.signal-page-header {
  max-width: 1140px;
  margin: auto;
}
.signal-page-content {
  margin-bottom: 30px;
}
</style>
