<template>
   <div class="slotClass">
      <div>
          111
          <slot name="aaClass" v-for="(item) in table" :aa="item"></slot>
          333
      </div>
   </div>
</template>

<script>

export default {
    name: 'edit-list-lab',
    props:{
        table: {
            type: Array,
            default: function(){return []}
        }
    },
    created() {
        this.$nextTick(()=>{
            console.log('table', this.table)
        });
    },
    data(){
        return {
        }
    },

    methods: {
        
    }
}
</script>

<style lang='stylus' rel='stylesheet/stylus'>
</style>