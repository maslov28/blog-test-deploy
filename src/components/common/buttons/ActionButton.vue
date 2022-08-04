<template>
  <a :class="color" class="action-button"  href="#"><slot></slot></a>
</template>

<script>
export default {
  props: {
    color: String,
  }
}
</script>

<style>
.action-button {
  padding: 20px 59px;
  border-radius: 30px;
  display: inline-block;
  font-weight: 600;
  line-height: 20px;
}
</style>