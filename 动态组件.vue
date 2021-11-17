<template>
  <div v-for="val in componentsData" :key="val.id">
    <component :is="val.type" />
  </div>
</template>
<script>
import CustomTitle from './CustomTitle'
import CustomText from './CustomText'
import CustomImage from './CustomImage'

export default {
  data() {
    return {
      componentsData: [
        {
          id: 1,
          type: 'CustomTitle'
        },
        {
          id: 2,
          type: 'CustomText'
        },
        {
          id: 3
          type: 'CustomImage'
        }
      ]
    }
  }
}
</script>
