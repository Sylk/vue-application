<template>
<header>
    <ul style="list-style-type: none; margin: 0; padding: 0; overflow: hidden; background-color: #333333;">
        <li style="float: left;">
            <h1 style="color:white;">Vue Application</h1>
        </li>    
        <li v-for="link in links" style="float: left;">
            <a :href="link" style="display: block; color: white; text-align: center; padding: 16px; text-decoration: none;">
                {{link}}
            </a>
        </li>
    </ul>    
</header>  
</template>

<script>

export default {
  props: {
    // links: Array
  },
  data: function () {
      return {links: ['Home','About','Contact']}
  }
};
</script>