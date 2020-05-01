<template>
<button @click="onClick" class="Button">
  <slot>Button</slot>
</button>
</template>

<script>
export default {
  props: {
    onClick: {
      type: Function,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
$color: #de8585;
.Button {
  background: $color;
  border: none;
  color: #fff;
  cursor: pointer;
  font-size: 0.75rem;
  padding: 10px 25px;
  margin: 0.5em;
  text-transform: uppercase;
  transition: background .2s ease-in-out;

  &:hover {
    background: darken($color, 20);
  }

  &:disabled {
    opacity: 0.5;
  }
}
</style>