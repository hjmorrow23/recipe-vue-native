<template>
  <app-navigator></app-navigator>
</template>
<script>
import { createAppContainer, createStackNavigator } from 'vue-native-router'

import Home from './src/views/Home.vue'
import Recipe from './src/views/Recipe.vue'

const StackNavigator = createStackNavigator(
  {
    Home: Home,
    Recipe: Recipe,
  },
  {
    initialRouteName: 'Home',
  }
)

const AppNavigator = createAppContainer(StackNavigator)

export default {
  components: { AppNavigator },
}
</script>
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
