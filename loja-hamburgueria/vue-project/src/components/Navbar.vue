<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img src="img/logo.png" :alt="alt" id="logo">
        </router-link>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/pedidos">Pedidos</RouterLink> 
    </div> 
    
</template>

<script>
export default {
   name: 'Navbar',
   props: ["logo", "alt"]
}
</script>

<style>
#nav{
  background: #222;
  border-bottom: 4px solid #111;
  padding:15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#nav #logo-url{
    margin:auto;
    margin-left: 0;
} 

#logo{
    width: 40px;
    height: 40px;
}

#nav a{
    color: yellow;
    text-decoration: none;
    margin: 12px;
}

</style>