<template>
<div class="benefit-item">
  <div class="benefit-item-container">
    <div>
      <slot name="image" />
    </div>
    <h3 class="benefit-item-title">
      {{ titleText }}
    </h3>
    <div class="benefit-item-des">
      {{ description  }}
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'BenefitItem',
  props: {
    titleText: {
      type: String,
      default: '',
    },
    description: {
      type: String,
      default: '',
    },
  },
}
</script>
<style>
.benefit-item-container {
  display: flex;
  align-items: center;
  flex-direction: column;
  background-color: #FFFFFF;
  border-radius: 16px;
  height: 540px;
  padding: 30px;
}
.benefit-item-title {
  color: #1b1b1b;
  font-size: 28px;
  font-weight: 800;
  line-height: 32px;
  margin-top: 18px;
  margin-bottom: 4px;
}
.benefit-item-des {
  font-size: 16px;
  font-weight: 400;
  line-height: 22px;
}
</style>
