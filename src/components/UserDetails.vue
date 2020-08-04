<template>
  <div class="names">
    {{`${name}-${lastname}`}}
    <button>-</button>
  </div>
</template>

<script>
export default {
  props: ["name", "lastname"],
};
</script>

<style scoped>
.names {
  height: 32px;
  padding: 6px;
  background: crimson;
  color: white;
}
</style>