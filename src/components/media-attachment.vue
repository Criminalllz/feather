<template>
  <div class="attachment">
    <img v-if="attachment.type == 'image'" :src="attachment.preview_url" :alt="attachment.alt">
  </div>
</template>

<script>
export default {
  props: ['attachment']
}
</script>

<style scoped>
.attachment {
  float: left;
}

img {
  height: 300px;
  padding-right: 4px;
}
</style>
