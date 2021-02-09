<template>
  <view>
    <text>Recipe</text>
    <button title="Go to Home screen" @press="goToHomeScreen"></button>
  </view>
</template>

<script>
export default {
  props: {
    navigation: {
      type: Object,
    },
  },
  methods: {
    goToHomeScreen() {
      this.navigation.navigate('Home')
    },
  },
}
</script>

<style lang="scss" scoped></style>
