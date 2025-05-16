<template>
  <div>
    <h2>Hallo, {{ name }}!</h2>
  </div>
</template>

<script>
export default {
  name: "HelloUser",
  props: {
    name: {
      type: String,
      required: true,
    },
  },
};
</script>
