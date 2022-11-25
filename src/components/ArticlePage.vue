<template>
   <article>
     <div>
       <button>SIGN-UP NOW!</button>
       <div>
         <h4>FOLLOW US</h4>
         <img src="@/img/footer-facebook.png" alt="error">
         <img src="@/img/footer-twitter.png" alt="error">
         <img src="@/img/footer-youtube.png" alt="error">
         <img src="@/img/footer-pinterest.png" alt="error">
       </div>
     </div>
   </article>
</template>

<script>
export default {
  name: 'ArticlePage',
};
</script>

<style  lang="scss" scoped>
   article{
     background-color: #303030;
     div{
       height: 4.6em;
       width: 1100px;
       margin: 0 auto;
       display: flex;

       align-items: center;
       button{
        border: 3px solid #0282F9;
        background-color:#303030 ;
        color: white;
        white-space: nowrap;
        padding: .5em .5em;
       }
       div{
        display: flex;
        color: #0282F9;
        justify-content: end;
        gap: 1em;
       }
     }
   }
</style>
