<template>
  <button class="zqkButton" :class="`zqk-button-${type}`">
    <span> <slot></slot> </span>
  </button>
</template>
<script>
export default {
  name: "ZqkButton",
  props: {
    type: {
      type: String,
      default: "default",
    },
  },
  data() {
    return {};
  },
  methods: {},
  components: {},
  computed: {},
  watch: {},
  created() {
  },
};
</script>
<style lang="scss" scoped>
.zqkButton {
  display: inline-block;
  line-height: 1;
  white-space: nowrap; //不换行
  cursor: pointer; //  小手
  background: #ffffff;
  border: 1px solid #dcdfe6;
  color: #606266;
  -webkit-appearance: none; //去除系统默认appearance的样式
  text-align: center;
  box-sizing: border-box;
  outline: none; //定义无轮廓
  margin: 0;
  transition: 0.1s;
  font-weight: 500;
  //禁止元素的文字被选中
  -moz-user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  padding: 12px 20px;
  font-size: 14px;
  border-radius: 4px;
  &:hover,
  &:hover {
    color: #409eff;
    border-color: #c6e2ff;
    background-color: #ecf5ff;
  }
}
.zqk-button-primary {
  color: #fff;
  background-color: #409eff;
  border-color: #409eff;
  &:hover,
  &:focus {
    background: #66b1ff;
    background-color: #66b1ff;
    color: #fff;
  }
}
.zqk-button-success {
  color: #fff;
  background-color: #67c23a;
  border-color: #67c23a;
  &:hover,
  &:focus {
    background: #85ce61;
    background-color: #85ce61;
    color: #fff;
  }
}
.zqk-button-info {
  color: #fff;
  background-color: #909399;
  border-color: #909399;
  &:hover,
  &:focus {
    background: #a6a9ad;
    background-color: #a6a9ad;
    color: #fff;
  }
}
.zqk-button-warning {
  color: #fff;
  background-color: #e6a23c;
  border-color: #e6a23c;
  &:hover,
  &:focus {
    background: #ebb563;
    background-color: #ebb563;
    color: #fff;
  }
}
.zqk-button-danger {
  color: #fff;
  background-color: #f56c6c;
  border-color: #f56c6c;
  &:hover,
  &:focus {
    background: #f78989;
    background-color: #f78989;
    color: #fff;
  }
}
</style>
