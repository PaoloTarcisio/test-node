<script >

/*
    1) Importo il componente
        es. import *nome file* from *percorso file*

    2) Dichiarazione del componente all'interno dell'oggetto
        es. components:{
            *nome file*
        }

    3) Aggiungo un tag con il nome del componente all'interno del template (template ha SOLO UN FIGLIO DIRETTO)
*/ 

import AppHeader from './components/AppHeader.vue'; // 1


export default {
  data() {
    return { 
      count: 0 
    }
  },
  components: {             //2
    AppHeader
  }
}
</script>

<template>

    <div>
        <AppHeader/>               
        <h1>Hello World</h1>
    
        <p>
            {{ count }}
        </p>
    
        <button @click="count++">
            Cliccami!
        </button>
    </div>

</template>

<style scoped>

</style>