<template>
  <button :class="'button ' + this.color">
    Click Me!
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
    isOutline: Boolean,
  },
  computed: {},
  data() {
    return {

    };
  },
};
</script>

<style lang="scss" scoped>
.button {
  color: white;
  background-color: lightblue;
  height: 20px;
  width: 75px;
  border-radius: 10px;

  &.green {
    background-color: lightseagreen;
  }

  &.red {
    background-color: firebrick;
  }

  &.purple {
    background-color: purple;
  }

  &.yellow {
    color: black;
    background-color: yellow;
  }

  &.gray {
    background-color: gray;
  }
}
</style>
