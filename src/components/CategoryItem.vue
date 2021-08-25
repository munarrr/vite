<template>
  <a href="#" :class="classes">{{category}}</a>
</template>

<script>


export default {
  props:['category','isActive'],

computed:{
  classes() {
    const classes = ['px-3',' py-1', 'transition'  ,'border' , 'rounded-full']
  return this.isActive
  ? [...classes,'hover:bg-gray-500', 'text-white' ,'bg-gray-600', 'border-gray-700']:[...classes,'hover:bg-gray-200', 'bg-gray-100', 'border-gray-300']
    }
}
}
</script>

<style scoped>

</style>