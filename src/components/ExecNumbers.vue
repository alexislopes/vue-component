<template>
  <div>
    <p>{{one}} * {{two}} = {{one * two}}</p>
    <p>{{one}} - {{two}} = {{one - two}}</p>
    <p>{{one}} + {{two}} = {{Number(one) + Number(two)}}</p>
  </div>
</template>

<script>
export default {
  props: {
    one: Number,
    two: Number
  }
};
</script>

<style>
</style>

