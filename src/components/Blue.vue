<template>
    <div>
      <slot name="blueContent">
        <h1>Blue content</h1>
        <p><span class="label label-primary">Blue</span> Lorem ipsum</p>
      </slot>
    </div>
</template>

<script>

</script>

<style scoped>
    div {
        border: 1px solid blue;
        background-color: lightblue;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>
