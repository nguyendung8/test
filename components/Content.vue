<template>
<div class="content">
  <div class="first-content">
    <IntroduceItem
      title-text="Chia sẻ Không Ngại Lỗ hổng"
      first-text="Phương thức mã hoá hai đầu cuối tân tiến (được hỗ trợ bởi Giao thức Signal mã nguồn mở) để giữ các cuộc trò chuyện của bạn được an toàn"
      second-text="Chúng tôi không đọc được tin nhắn của bạn hoặc nghe được cuộc gọi của bạn, và cũng không ai khác có thể"
      third-text="Mọi tin nhắn, mọi cuộc gọi, mọi lúc."
    >
      <template v-slot:image>
        <img class="introduce-image" src="../assets/image/introduceimg1.jpg" />
      </template>
    </IntroduceItem>
  </div>
  <div class="second-content">
    <div class="second-content-container">
      <h1 class="second-content-title mb-6">Đứng vững trước các mối đe dọa đối với thông tin liên lạc riêng tư và an toàn</h1>
      <div class="text-base font-normal mb-2">Cung cấp cho mọi người ở khắp mọi nơi một công cụ để liên lạc riêng tư thực sự</div>
      <div class="text-base font-normal mb-2">Quyền riêng tư không phải là một chế độ tùy chọn — đó đơn giản là cách Signal hoạt động</div>
      <div class="text-base font-normal mb-2">Hàng triệu người trên toàn thế giới dựa vào Signal mỗi ngày để liên lạc an toàn và riêng tư</div>
      <img class="second-container-image mt-4 mb-7" src="../assets/image/introduceimg2.jpg" />
      <a class="install-btn" href="https://signal.org/vi/download/" target="blank">TRẢI NGHIỆM MIỄN PHÍ NGAY</a>
    </div>
  </div>
  <div class="third-content">
    <IntroduceItem
      title-text="Không quảng cáo. Không theo dõi. Không đùa."
      first-text="Signal không có bất kỳ mục quảng cáo, bên quảng cáo thứ ba nào"
      second-text="Signal không theo dõi người dùng."
      third-text="Hãy cứ yên tâm tập trung cho những khoảnh khắc quan trọng với bạn với những người quan trọng."
    >
      <template v-slot:image>
        <img class="introduce-image" src="../assets/image/introduceimg3.png" />
      </template>
    </IntroduceItem>
  </div>
  <div class="fourth-content">
    <div class="fourth-content-container">
      <h1 class="second-content-title mb-6">Lợi ích khi sử dụng</h1>
      <div class=" flex flex-wrap gap-6 mb-6">
        <div class="flex-1">
          <BenefitItem
            title-text="Nói bất cứ điều gì"
            description="Chia sẻ miễn phí văn bản, tin nhắn thoại, hình ảnh, video, ảnh động và tập tin. Signal sử dụng kết nối dữ liệu di động của bạn để bạn có thể tránh các phí SMS và MMS."
          >
            <template v-slot:image>
              <img class="benefit-item-image" src="../assets/image/demo1.png" />          
            </template>
          </BenefitItem>
        </div>
        <div class="flex-1">
          <BenefitItem
            title-text="Nói chuyện Tự do"
            description="Thực hiện các cuộc gọi thoại và video cực rõ với bất cứ ai sống bên kia thành phố, hoặc bên kia bờ đại dương, mà không phải tốn phí gọi đường dài."
          >
            <template v-slot:image>
              <img class="benefit-item-image" src="../assets/image/demo2.png" />          
            </template>
          </BenefitItem>
        </div>
      </div>
      <div class="flex flex-wrap gap-6 mb-6">
        <div class="flex-1">
          <BenefitItem
            title-text="Quyền Riêng Tư & Nhãn Dán"
            description="Thêm một lớp biểu cảm cho các cuộc trò chuyện của bạn với nhãn dán được mã hoá. Bạn cũng có thể tạo và chia sẻ các bộ nhãn dán của riêng mình."
          >
            <template v-slot:image>
              <img class="benefit-item-image" src="../assets/image/demo3.png" />          
            </template>
          </BenefitItem>
        </div>
        <div class="flex-1">
          <BenefitItem
            title-text="Gặp nhau qua Nhóm"
            description="Trò chuyện nhóm giúp bạn giữ liên lạc với gia đình, bạn bè, và đồng nghiệp một cách dễ dàng."
          >
            <template v-slot:image>
              <img class="benefit-item-image" src="../assets/image/demo4.png" />          
            </template>
          </BenefitItem>
        </div>
      </div>
      <a class="install-btn" href="https://signal.org/vi/download/" target="blank">TRẢI NGHIỆM MIỄN PHÍ NGAY</a>
    </div>
  </div>
  <div class="fifth-content">
    <h1 class="second-content-title mt-5 text-center">Vì sao nên sử dụng Signal</h1>
    <IntroduceItem
    first-text="Miễn phí cho tất cả mọi người"
    second-text="Signal là một tổ chức phi lợi nhuận độc lập,không có liên kết với các công ty công nghệ lớn và không bao giờ bị mua bởi các công ty này"
    third-text="Việc phát triển Signal được hỗ trợ bởi các khoản trợ cấp và khoản ủng hộ từ các cá nhân như bạn"
    :show-button="false"
    :show-donate="true"
  >
    <template v-slot:image>
      <img class="introduce-image" src="../assets/image/introduceimg4.png" />
    </template>
  </IntroduceItem>
  </div>
</div>
</template>

<script>
import IntroduceItem from './IntroduceItem.vue';
import BenefitItem from './BenefitItem.vue';

export default {
  name: 'Content',

  components: {
    IntroduceItem,
    BenefitItem,
  },
}
</script>
<style>
.introduce-image {
  width: 660px;
  height: 540px;
  border-radius: 10px;
}
.benefit-item-image {
  width: 370px;
  height: 370px;
}
.second-content {
  background-color: #FAFAFA;
}
.second-content-container {
  padding: 60px 16px 32px;
  max-width: 1140px;
  margin: auto;
  text-align: center;
}
.second-content-title {
  font-size: 28px;
  font-weight: 700;
  color: #3A76F0;
}
.third-content {
  background-color: #FFF5E7;
}
.fourth-content {
  background-color: #F0FBFF;
}
.fourth-content-container {
  padding: 60px 16px 32px;
  max-width: 1140px;
  margin: auto;
  text-align: center;
}
</style>
