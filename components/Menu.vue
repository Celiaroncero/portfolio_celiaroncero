<template>
  <div class="menu">
    <div class="menuitems">
      <NuxtLink to="/">Proyectos</NuxtLink>
      <NuxtLink to="pagina2">Sobre mí</NuxtLink>
      <NuxtLink to="pagina3">Contacto</NuxtLink>
      <NuxtLink to="pagina4">Galeria</NuxtLink>
      
    </div>
  </div>
</template>

<style lang="scss">
.menu{
  background: black;
  height: 90px;
  display: flex;
  align-items: center;
  justify-content: center;

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
@media screen and (max-width: 600px) {
  
.menu{
  background: black;
  height: 90px;
  display: flex;
  align-items: center;
  justify-content: center;

  .menuitems{
    padding: 2em;
    
    
    a{
      color: white;
      text-decoration: none ;
      padding: 0.7em;
      font-size: 0.8em;


    }
}
}
 

}

</style>
