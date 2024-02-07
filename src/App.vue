<script>
import CompHeader from './components/CompHeader.vue'
import CompMain from './components/CompMain.vue'
import CompFooter from './components/CompFooter.vue'

export default{
    components:{
        CompHeader,
        CompMain,
        CompFooter,
    }
}
</script>

<!-- ----------------------------------------------------------------------------- -->

<template>


<CompHeader/>
<!---->
<CompMain/>
<!---->
<CompFooter/>


</template>

<!-- ----------------------------------------------------------------------------- -->

<style lang="scss">
// percorso per il file general.scss
@use './styles/general.scss' as *;

</style>
