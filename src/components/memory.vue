<template>
<div class="text-center">

<div  class="test"><slot name="heading"></slot></div>

<div  class="test"><slot name="content"></slot></div>
<div class="test"> <slot name="author"> No content came here</slot> </div>

</div></template>


<script>


export default{

}
</script>

<style scoped>
div.test {
    border: 1px solid #ccc;
    box-shadow: 1px 1px 2px #666;
    padding: 20px 20px;
    margin-top: 20px;

}
</style>