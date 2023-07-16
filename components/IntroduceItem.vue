<template>
<div class="introduce-item">
  <div class="introduce-item-container">
    <div class="introduce-item-text flex-1">
      <div class="introduce-item-title"> {{ titleText }} </div>
      <div class="introduce-item-des">
        <div class="flex gap-4 mb-4">
          <div>
            <font-awesome-icon :icon="['fas', 'check']"  class="checkbox-icon"/>
          </div>
          <span class="text-base"> {{ firstText }} </span>
        </div>
        <div class="flex gap-4 mb-4">
          <div>
            <font-awesome-icon :icon="['fas', 'check']"  class="checkbox-icon"/>
          </div>
          <span class="text-base"> {{ secondText }} </span>
        </div>
        <div class="flex gap-4 mb-4">
          <div>
            <font-awesome-icon :icon="['fas', 'check']"  class="checkbox-icon"/>
          </div>
          <span class="text-base"> {{ thirdText }} </span>
        </div>
        <div v-if="showButton" class="mt-12 mb-3">
          <a class="install-btn" href="https://signal.org/vi/download/" target="blank">TRẢI NGHIỆM MIỄN PHÍ NGAY</a>
          <img class="qr-img" src="../assets/image/qr.png" />
        </div>
        <div v-if="showDonate" class="mt-12 mb-3">
          <a class="donate-btn" href="https://signal.org/vi/donate/" target="blank">Ủng hộ Signal</a>
        </div>
      </div>
    </div>
    <div class="flex-1">
      <slot name="image" />
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'IntroduceItem',
  props: {
    titleText: {
      type: String,
      default: '',
    },
    firstText: {
      type: String,
      default: '',
    },
    secondText: {
      type: String,
      default: '',
    },
    thirdText: {
      type: String,
      default: '',
    },
    description: {
      type: String,
      default: '',
    },
    showButton: {
      type: Boolean,
      default: true,
    },
    showDonate: {
      type: Boolean,
      default: false,
    }
  },
}
</script>
<style>
.introduce-item-container {
  padding: 60px 16px 32px;
  max-width: 1140px;
  margin: auto;
  display: flex;
  gap: 30px;
}
.introduce-item-title {
  font-size: 28px;
  font-weight: 700;
  color: #3A76F0;
  margin-bottom: 24px;
}
.checkbox-icon {
  width: 28px;
  height: 28px;
  background-color: #F0FBFF;
  color: #3A76F7;
  border-radius: 50%;
}
.qr-img {
  width: 150px;
  margin-top: 20px;
}
.donate-btn {
  background-color: #fff;
  border-radius: 8px;
  border: 2px solid #2c6bed;
  color: #2c6bed;
  font-size: 20px;
  font-weight: 700;
  cursor: pointer;
  justify-content: center;
  padding-bottom: calc(0.5em - 1px);
  padding-left: 1em;
  padding-right: 1em;
  padding-top: calc(0.5em - 1px);
  text-align: center;
  white-space: nowrap;
}
</style>
