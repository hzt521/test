<template>
  <div class="nav-bar">
    <div class="left">
      <!-- 预留插槽 -->
      <slot name="left"></slot>
      </div>
    <div class="center"> <slot name="center"></slot> </div>
    <div class="right"> <slot name="right"></slot> </div>

  </div>
</template>

<script>
export default{
  name:"NavBar"
  
}
</script>

<style scoped>
.nav-bar{
  display:flex;
  height:44px;
  line-height:44px;
  text-align:center;
  /* 加阴影 */
  box-shadow: 0 1px 1px rgba(100,100,100,.1);
  
}
.left,.right{
  width:60px;
 
}
.center{
  /* 将除左，右两部分外剩余部分全部占据 */
  flex:1;
}

</style>
