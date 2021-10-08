<template>
  <div id="app">  <!--Na linha 2,temos a tag h1 que deverá exibir o conteúdo da propriedade titulo,definida na linha 11  -->
    <h1>{{ titulo }}</h1>
  </div>
</template>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<script>
    var app = new Vue({
        el:'app',
        data:{
            titulo:'Página de Cursos
        }
    });



</script>
  <!-- A instancia Vue esta diretamente ligada a div de id app  -->
  <!-- Para que o data bind funcione, as tags com as quais desejamos ligar os dados devem estar no interior dessa div -->


 
---------------------------------------------------------------------------------------------------------------------------
<template>
  <div id="app">  <!--Na linha 2,temos a tag h1 que deverá exibir o conteúdo da propriedade titulo,definida na linha 11  -->
    <h1>{{ titulo }}</h1>
    <input type="text" v-model="titulo">
  </div>
</template>
<script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
<script>
    var app = new Vue({
        el:'app',
        data:{
            titulo:'Página de Cursos
        }
    });



</script>

 <!-- Sempre que o conteudo do input for alterado, essa mudança será refletida na propriedade TITULO e,conseguentemente em todos os elementos visuais
 que estiverem ligados a ela,como a tag h1,adicionada anteriormente-->