<template>
    <button :style="{background: colour}" class='btn'>{{ text }}</button>
</template>

<script>
  export default {
    name: 'Button',
    props: {
        colour: String,
        text: String
    }
  }
</script>
