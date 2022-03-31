<template>
  <div class="counter">
    <button class="counter-decrease" @click="decrease">-</button>
    <div class="counter-number">{{ countNum }}</div>
    <button class="counter-increase" @click="increase">+</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      countNum: 0,
    };
  },
  methods: {
    decrease() {
      if (this.countNum >= 1) {
        this.countNum--;
      } else {
        return;
      }
    },
    increase() {
      if (this.countNum <= 9) {
        this.countNum++;
      } else {
        return;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.counter {
  @apply max-w-[200px] gap-4 p-4 inline-flex items-center justify-between bg-slate-50 rounded-xl border border-slate-200;

  &-number {
    @apply w-10 text-center;
  }

  &-decrease,
  &-increase {
    @apply flex items-center justify-center w-6 h-6 rounded pb-1 bg-slate-200 hover:bg-slate-300 active:bg-white text-slate-700;
  }
}
</style>