<template>
  <view>
    <text>Hey Yall</text>
    <button title="Go to Recipe screen" @press="goToRecipeScreen"></button>
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
    goToRecipeScreen() {
      this.navigation.navigate('Recipe')
    },
  },
}
</script>

<style lang="scss" scoped></style>
