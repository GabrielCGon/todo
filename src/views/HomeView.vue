<template>
  <v-content > 
      <header-comp/>
        <v-content id="theme">
            <div>
                <h1
                class="formatacao"
                >
                    KJ すべて
                </h1>
            </div> 

        </v-content> 
  </v-content>
</template>


<script>
import HeaderComp from '@/components/HeaderComp.vue'
export default {
  components: { HeaderComp },   
}
</script>
<style scoped>
  #theme{
    background: linear-gradient(to right,#7E0F4B, #1A5865);
    height: 915px;
  }

.formatacao{
    text-align: center;
    color: white;
    padding-top: 4%;

}
</style>