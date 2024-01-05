<template>
  <header>
    
  </header>

  <main>
    
    <ul>
    <li v-for= "task  in Zadachi" :key="task.link">
        <p @click="task.show=!task.show">{{task.title}}</p>
            
              <component v-if="task.show" v-bind:is="task.link"></component>
       

        </li>
      </ul>
  </main>
</template>


<script setup lang="ts">
import { reactive,  } from 'vue'

import ZadachaP1 from "./components/ZadachaP1.vue";
import ZadachaP2 from "./components/ZadachaP2.vue";
import ZadachaP3 from "./components/ZadachaP3.vue";
import ZadachaP4 from "./components/ZadachaP4.vue";
import ZadachaP5 from "./components/ZadachaP5.vue";
import ZadachaP6 from "./components/ZadachaP6.vue";
import ZadachaP7 from "./components/ZadachaP7.vue";
import ZadachaP8 from "./components/ZadachaP8.vue";
import ZadachaP9 from "./components/ZadachaP9.vue";
import ZadachaP10 from "./components/ZadachaP10.vue";
import ZadachaP11 from "./components/ZadachaP11.vue";
import ZadachaP12 from "./components/ZadachaP12.vue";
import ZadachaP13 from "./components/ZadachaP13.vue";
import ZadachaP14 from "./components/ZadachaP14.vue";
import ZadachaP15 from "./components/ZadachaP15.vue";
import ZadachaP16 from "./components/ZadachaP16.vue";
import ZadachaP17 from "./components/ZadachaP17.vue";
// import ZadachaP18 from "./components/ZadachaP18.vue";
// import ZadachaP19 from "./components/ZadachaP19.vue";
import ZadachaP20 from "./components/ZadachaP20.vue";
import ZadachaP21 from "./components/ZadachaP21.vue";


const Zadachi = reactive([
  {
    show:true,
    title:'Задача 1',
    link: ZadachaP1
  },
  {
    show:false,
    title:'Задача 2',
    link: ZadachaP2 
  },
  {
    show:false,
    title:'Задача 3',
    link: ZadachaP3
  },
  {
    show:false,
    title:'Задача 4',
    link:ZadachaP4
  },
  {
    show:false,
    title:'Задача 5',
    link:ZadachaP5
  },
  {
    show:false,
    title:'Задача 6',
    link:ZadachaP6
  },
  {
    show:false,
    title:'Задача 7',
    link:ZadachaP7
  },
  {
    show:false,
    title:'Задача 8',
    link:ZadachaP8
  },
  {
    show:false,
    title:'Задача 9',
    link:ZadachaP9
  },
  {
    show:false,
    title:'Задача 10',
    link:ZadachaP10
  },
  {
    show:false,
    title:'Задача 11',
    link:ZadachaP11
  },
  {
    show:false,
    title:'Задача 12',
    link:ZadachaP12
  },
  {
    show:false,
    title:'Задача 13',
    link:ZadachaP13
  },
  {
    show:false,
    title:'Задача 14',
    link:ZadachaP14
  },
  {
    show:false,
    title:'Задача 15',
    link:ZadachaP15
  },
  {
    show:false,
    title:'Задача 16',
    link:ZadachaP16
  },
  {
    show:false,
    title:'Задача 17',
    link:ZadachaP17
  },
  /* {
    show:false,
    title:'Задача 18',
    link:ZadachaP18
  }, */
  /* {
    show:false,
    title:'Задача 19',
    link:ZadachaP19
  }, */
  {
    show:false,
    title:'Задача 20',
    link:ZadachaP20
  },
  {
    show:false,
    title:'Задача 21',
    link:ZadachaP21
  },
] ) 

</script>


