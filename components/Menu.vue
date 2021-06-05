<template>
  <div class="menu">
    <div class="menuitems">
      <NuxtLink to="/">Proyectos</NuxtLink>
      <NuxtLink to="pagina2">Sobre mí</NuxtLink>
      <NuxtLink to="pagina3">Contacto</NuxtLink>
      
    </div>
  </div>
</template>

<style lang="scss">
.menu{
  background: black;
  height: 90px;
  align-items: center;

  .menuitems{
    padding: 2em;
    
    
    a{
      color: white;
      text-decoration: none ;
      padding: 1em;
      font-size: 1.2em;

    }
}
}

</style>
