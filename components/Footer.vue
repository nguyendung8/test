<template>
<div class="footer">
  <div class="footer-container">
    <div class="footer-logo">
      <div>
        <a href=""> <img class="footer-img" src="../assets/image/logo.png" /> </a>
      </div>
      <div class="footer-logo-des">Signal is a registered trademark in the United States and other countries.</div>
      <div class="footer-logo-copyright">Copyright © 2013–2023 Signal, a 501c3 nonprofit.</div>
    </div>
    <ul class="company-about">
      <li class="company-about-item-title">
        TỔ CHỨC
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/donate/" target="blank">Ủng hộ Signal</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/workworkwork/" target="blank">Nghề nghiệp</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/legal/#terms-of-service" target="blank">Điều khoản sử dụng</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/legal/#privacy-policy"  target="blank">Chính sách bảo mật</a>
      </li>
    </ul>
    <ul class="company-about">
      <li class="company-about-item-title">
        TẢI XUỐNG
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/download/android/" target="blank">Android</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/download/ios/" target="blank">iPhone & iPad</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/download/macos/" target="blank">Mac</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/download/windows/"  target="blank">Windows</a>
      </li>
      <li class="company-about-item">
        <a href="https://signal.org/vi/download/linux/"  target="blank">Linux</a>
      </li>
    </ul>
    <ul class="company-about">
      <li class="company-about-item-title">
        HỖ TRỢ
      </li>
      <li class="company-about-item">
        <a href="https://support.signal.org/hc/en-us" target="blank">Trung tâm hỗ trợ</a>
      </li>
      <li class="company-about-item">
        <a href="https://community.signalusers.org/" target="blank">Cộng đồng</a>
      </li>
      <li class="company-about-item">
        Email: press@signal.org
      </li>
    </ul>
    <ul class="company-about">
      <li class="company-about-item-title">
        MẠNG XÃ HỘI 
      </li>
      <li class="company-about-item">
        <a class="text-2xl" href="https://github.com/signalapp" target="blank">
          <font-awesome-icon :icon="['fab', 'github']"  class="icon-footer"/>
        </a>
      </li>
      <li class="company-about-item">
        <a class="text-2xl twitter" href="https://twitter.com/i/flow/login?redirect_after_login=%2Fsignalapp" target="blank">
          <font-awesome-icon :icon="['fab', 'twitter']" class="icon-footer" />
        </a>
      </li>
      <li class="company-about-item">
        <a href="https://www.instagram.com/signal_app/" target="blank">
          <!-- <font-awesome-icon :icon="['fab', 'instagram']" /> -->
          <img class="instagram" src="../assets/image/Instagram_logo_2022.svg" />
        </a>
      </li>
    </ul>
  </div>
</div>
</template>

<script>
export default {
  name: 'Footer',
}
</script>
<style>
.footer {
  width: 100%;
  background-color: #F0FBFF;
}
.footer-container {
  padding: 30px 32px;
  max-width: 1140px;
  margin: auto;
  display: flex;
  justify-content: space-around;
}
.footer-logo {
  width: 395px;
}
.footer-img {
  width: 205px;
  height: 59px;
  margin-bottom: 33px;
}
.footer-logo-des {
  margin-bottom: 33px;
}
.company-about {
  margin-top: 15px;
}
.company-about-item-title {
  font-size: 16px;
  font-weight: 700;
  margin-bottom: 24px;
  color: #3A76F0;
}
.company-about-item {
  margin-bottom: 24px;
}
.twitter {
  color: #1C96E8;
}
.instagram {
  width: 24px;
}
.company-about-item:hover {
  text-decoration: underline;
}
.icon-footer {
  width: 24px;
  height: 24px;
}
</style>
