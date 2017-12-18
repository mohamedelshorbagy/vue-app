<template>

<div class="container">
  <div class="row">
    <div class="col-xs-10 col-xs-offset-1">

    <navbar-app :navbarList="navbarList"></navbar-app>

    <post-app>
        <ul class="list-group">
          <li class="list-group-item">Name : Mohamed Elshorbagy</li>
          <li class="list-group-item">Age : 21</li>
        </ul>
    </post-app>


    <input-app type="input" elementType="text" pc="username"></input-app>
    <input-app type="textarea" rows="10" cols="30" pc="Message"></input-app>
    <input-app type="select" :elOpts="elementsOptions"></input-app>



    </div>
  </div>


</div>

</template>

<script>
  import Input from './components/Input.vue';
  import Navbar from './components/Navbar.vue';
  import Post from './components/Post.vue'
export default {
  components:{
    inputApp: Input,
    navbarApp: Navbar,
    postApp:Post
  },
  data() {
    return {
      name:'Mohamed',
      navbarList:['Home','About','Contact'],
      elementsOptions:['First','Second','Third','Fourth','Fifth']
    }
  }
}
</script>

<style>

hr {
  border-color:rgb(52, 73, 94);
}

</style>
