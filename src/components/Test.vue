<template>
  <div class = "lst">
    <ul class="items">
      <li>{{name}}</li>
    </ul>
  </div>
</template>

<script>
export default{
  name:'Test',
  props:["name"]
}
</script>