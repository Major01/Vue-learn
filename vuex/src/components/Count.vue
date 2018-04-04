<template>
  <div>
      <h2>{{msg}}</h2><hr>
      <h3>{{count}}</h3>
      <p><button @click="add">增加</button><button @click="$store.commit('jian')">减少</button></p>
  </div>
</template>

<script>
    import store from '@/vuex/store';
    import {mapState, mapMutations} from 'vuex';
    export default {
        data(){
            return{
                msg:'Hello Vuex'
            }
        },
        // 第一种取state值的方法
        // computed:{
        //     count(){
        //         return this.$store.state.count;
        //     }
        // },
        // 第二种取state值方法
            computed: mapState(['count']),
            methods: mapMutations(['add','jian']),
        store
    }
</script>
