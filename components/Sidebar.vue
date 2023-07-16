<template>
<div class="sidebar">
  <div class="sidebar-container">
    <div class="sidebar-description mb-8">
      <h1 class="slogan text-4xl font-bold mb-6">Nền tảng <span class="text-strong">Nói chuyện tự do & thoải mái</span></h1>
      <span class="des">Các tính năng hỗ trợ quyền riêng tư ngoài mong đợi, kết hợp với những tính năng nhắn tin bạn mong chờ</span>
      <div class="mt-12 mb-3">
        <a class="nav-link install-btn" href="https://signal.org/vi/download/" target="blank">TRẢI NGHIỆM MIỄN PHÍ NGAY</a>
      </div>
      <span>Nếu bạn đã tải xuống? <a href=""> <strong class="text-strong"> Hãy thử ngay -> </strong> </a> </span>
    </div>
    <div class="sidebar-image">
    <img class="sidebar-image1" src="../assets/image/phone1.png" />
    <img class="sidebar-image2" src="../assets/image/phone2.png" />
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'Sidebar',
}
</script>
<style>
.sidebar {
  width: 100%;
  height: 1036px;
  background-color: #F0FBFF;
}
.sidebar-container {
  padding: 60px 16px 32px;
  max-width: 1140px;
  margin: auto;
}
.text-strong {
  color: #3A76F0;
}
.sidebar-description {
  text-align: center;
}
.sidebar-image {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 60px;
}
.sidebar-image1 {
  width: 350px;
  height: 100%;
}
.sidebar-image2 {
  width: 368px;
  height: 100%;
}
</style>
