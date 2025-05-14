<template>
    <div>
        <Navigation v-if="!isMotionDesignPage"/>
        <NuxtPage />
    </div>
</template>

<script>
export default {
  computed: {
    // Check if the current route name is 'motiondesign'
    isMotionDesignPage() {
      return this.$route.name === 'motiondesign'
    }
  }
}
</script>