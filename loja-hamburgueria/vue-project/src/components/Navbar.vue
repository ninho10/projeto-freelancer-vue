<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img src="logo" :alt="alt" id="logo">
        </router-link>
        <RouterLink to="/">Home</RouterLink>|
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

#logo-url{
    margin:auto;
    margin-left: 0;
} 


</style>