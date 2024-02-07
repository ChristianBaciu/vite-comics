<script>
import CompHeader from './components/CompHeader.vue'
import CompMain from './components/CompMain.vue'

export default{
    components:{
        CompHeader,
        CompMain,
    }
}
</script>


<!-- ----------------------------------------------------------------------------- -->



<template>

<CompHeader/>
<CompMain/>



</template>


<!-- ----------------------------------------------------------------------------- -->


<style lang="scss">
// percorso per il file general.scss
@use './styles/general.scss' as *;

</style>
