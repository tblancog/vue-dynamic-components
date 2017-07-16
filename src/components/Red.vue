<template>
    <div>
      <slot name="redContent">
        <h1>Red content</h1>
        <p><span class="label label-danger">Red</span> Lorem ipsum</p>
      </slot>
    </div>
</template>

<script>

</script>

<style scoped>
    div {
        border: 1px solid red;
        background-color: lightcoral;
        padding: 30px;
        margin: 20px auto;
        text-align: center
    }
</style>
