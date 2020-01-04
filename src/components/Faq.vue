<template>
  <div class="faq">
    <div class="container">
       <section class="section">
         <h1 class="title">FAQ</h1>
         <h2 class="subtitle is-4">risus pretium quam vulputate feugiat sed lectus</h2>

         <div class="columns" v-if="faqs && faqs.length">
           <div class="column is-one-third" v-for="faq of faqs">
             <div class="card">
               <div class="card content">
                 <p class="title-faq">{{faq.title}}</p>
                 <p class="answer">{{faq.body}}</p>
               </div>
             </div>
           </div>
         </div>
       </section>
    </div>
  </div>
</template>

<script>

import axios from 'axios';

export default {
  name: 'faq',
  data: () => ({
    faqs:[],
    errors:[]
  }),

  created(){
    axios.get('https://jsonplaceholder.typicode.com/posts')
      .then(response => {
        this.faqs = response.data.slice(0, 12);
      })
       .catch(e => {
         this.errors.push(e)
       })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.card.content
  padding: 1rem
.pd
  padding: 2.5em 0 1.5em 0
.title-faq
  font-size: 1.2em
  font-weight: 600
.answer
  margin-top: 1rem
  color: grey  
.columns
  flex-wrap: wrap  
</style>
