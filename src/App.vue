<template>
  <div id="app">
    <defaultNav/>
    <!--<keep-alive include="archive">-->
      <router-view/>
    <!--/keep-alive>-->
    <defaultFooter/>
  </div>
</template>

<script>
import defaultNav from '@/components/ebi/DefaultNav'
import defaultFooter from '@/components/ebi/DefaultFooter'
import '@/assets/js/iconfont.js'
export default {
  name: 'app',
  components:{
    defaultNav,
    defaultFooter
  }
}
</script>
<style type="text/css">
  html,body {
      min-width: 657px !important;
  }
  ul {
   list-style-type: disc;
   list-style-position: outside;
  }

  ol {
     list-style-type: decimal;
     list-style-position: outside;
  }

  ul ul, ol ul {
     list-style-type: circle;
     list-style-position: outside;

  }
  ol ol, ul ol {
     list-style-type: lower-latin;
     list-style-position: outside;

  }
  .page-container .ivu-select-dropdown-list{
    margin-left: 0 !important;
  }
  a{
        color:#495060;
    }
  a:hover{
      color:#5bc0be;
      border-bottom-style:dotted;
  }
  .masthead{
    background-color:white !important;
  }
  [type='text'], [type='password'], [type='date'], [type='datetime'], [type='datetime-local'], [type='month'], [type='week'], [type='email'], [type='number'], [type='search'], [type='tel'], [type='time'], [type='url'], [type='color'], textarea{
    margin: 0 !important;
  }
</style>

