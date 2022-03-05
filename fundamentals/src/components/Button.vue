<template>
    <button @click="onClick()" :style="{background: colour}" class='btn'>{{ text }}</button>
</template>

<script>
  export default {
    name: 'Button',
    props: {
        colour: String,
        text: String
    },
    methods: {
        onClick() {
            console.log('click')
            this.$emit('btn-click')
        }
    }
  }
</script>
