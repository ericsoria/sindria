<template>
  <div class="searchbar" >
    <input class="search_input" type="text" name="" placeholder="Search...">
    <a href="#" class="search_icon"><i class="fas fa-search"></i></a>
  </div>
</template>
<script>
  export default {
    name: 'list-creator'
  }
</script>
<style scoped>

  body,html{
    height: 100%;
    width: 100%;
    margin: 0;
    padding: 0;
    background: #e74c3c !important;
  }

  .searchbar{
    margin-bottom: auto;
    margin-top: auto;
    height: 60px;
    border-radius: 30px;
    padding: 10px;
    background: white;
    color: #e74c3c;
  }

  .search_input{
    color: white;
    border: 0;
    outline: 0;
    background: none;
    width: 0;
    caret-color:transparent;
    line-height: 40px;
    transition: width 0.4s linear;
  }


  .search_icon{
    height: 40px;
    width: 40px;
    float: right;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    color:white;
    text-decoration:none;
  }
</style>
