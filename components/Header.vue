<template>
<div class="header">
  <div style="width: 300px;">
   <a href=""> <img class="header-img" src="../assets/image/logo.png" /> </a>
  </div>
  <div class="navbar">
    <ul class="navbar-nav flex gap-4">
      <li class="nav-item active">
        <a href="">Trang chủ</a>
      </li>
      <li class="nav-item">
        <a href="https://community.signalusers.org/" target="blank">Cộng đồng</a>
      </li>
      <li class="nav-item">
        <a href="https://signal.org/blog/" target="blank">Blog</a>
      </li>
      <li class="nav-item">
        <a href="https://signal.org/vi/donate/" target="blank">Ủng hộ Signal</a>
      </li>
      <li class="nav-item-button">
        <a class="nav-link install-btn" href="https://signal.org/vi/download/" target="blank">Tải xuống</a>
      </li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  name: 'Header',
}
</script>
<style>
.header {
  height: 66px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.header-img {
  width: 205px;
  height: 59px;
}
.nav-item, .nav-item-button {
  padding: 20px 12px;
}
.nav-item:hover {
  color: #3A76F0;
}
.nav-item:active {
  color: #3A76F0;
}
.active {
  color: #3A76F0;
  border-bottom: 2px solid #3A76F0;
}
.install-btn {
  padding: 13px 19px;
  border-radius: 4px;
  background-color: #3A76F0;
  color: white;
}
.install-btn:hover {
  cursor: pointer;
}
</style>
