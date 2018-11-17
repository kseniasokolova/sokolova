<template>
  <div class="container">
    <header class="flex-container">
      <div class="social-block">
        <ul>
          <li><a href="#"><i class="fa fa-facebook"></i></a></li>
          <li><a href="#"><i class="fa fa-vk"></i></a></li>
          <li><a href="#"><i class="fa fa-instagram"></i></a></li>
          <li><a href="#"><i class="fa fa-youtube-play"></i></a></li>
        </ul>
      </div>
      <div class="links-block">
        <ul>
          <li>
            <nuxt-link to="/">Home</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/about">About</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/contacts">Contacts</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/gallery">Gallery</nuxt-link>
          </li>
           <li>
            <nuxt-link to="/test">Test</nuxt-link>
          </li>
        </ul>
      </div>
    </header>
    <nuxt/>
<footer>
   <p>© {{ year }} by Ksenia Sokolova </p>
</footer>
  </div>
</template>

<style>
body {
  margin: 0;
}
footer p {
  text-align: center;
}
  h1, h2 {


    font-family: 'Gruppo', cursive;


  }

  a {
    color: black
  }

  .container {
    max-width: 1000px;
    margin: 0 auto;
  }

  .flex-container {
    display: flex;
    flex-direction: row;
  }

  .fa-instagram:hover {
    color: #cd486b
  }

  .fa-youtube-play:hover {
    color: #ff0000
  }

  .fa-vk:hover {
    color: #45668e
  }

  .fa-facebook:hover {
    color: #3B5998
  }

  .social-block>ul>li {
    display: inline-block;
  }

  .social-block {
    width: 25%;
  }


  .social-block>ul>li {
    margin-right: 15px;
  }

  .links-block>ul>li {
    display: inline-block;
  }

  .links-block>ul>li a {
    text-decoration: none;
    text-transform: uppercase;
    padding-left: 10px;
  }

  .nuxt-link-exact-active {
    color: darkred;
  }

  .links-block {
    width: 75%;
    text-align: center;
  }

 @media only screen and (max-width: 480px) {
  .social-block {
    width: 100%;
    text-align: center;
  }
  .links-block {
    width: 0;
    visibility: hidden;
    height: 0;
  }
}

</style>


<script>
export default {
  data(){
    return {
      year: new Date().getFullYear()
    }
  }
}
</script>

