<template>
  <div class="home">
    <section class="hero is-danger">
      <div class="hero-body">
        <div class="container">
          <h1 class="card-title">
            {{heading}}
          </h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="subtitle is 4">{{subheading}}</h2>
          </div>
          <a class="button is-large is-warning" id="learn">Learn more</a>
        </div>
      </div>
  </section>

  <section class="section">
    <div class="container">
      <div class="columns pd is-desktop">
        <div class="column is-1 has-text-centered">
          <i class="fa fa-cog is-primary"></i>
        </div>
        <div class="column is-one-third-desktop">
          <p class="title"><strong>We provide superior logistics so that your bussiness can succeed in a crazy world.</strong></p>
        </div>  
        <div class="column">
          <p>Vel quam elementum pulvinar etiam non quam lacus suspendisse faucibus. Enim nulla aliquet porttitor lacus luctus accumsan tortor posuere. Eu non diam phasellus vestibulum lorem. Pharetra convallis posuere morbi leo urna. At risus viverra adipiscing at. Tempus egestas sed sed risus pretium quam vulputate. Ac feugiat sed lectus</p>
        </div>  
      </div>
    </div>

    <div class="columns pd">
      <div class="column">
        <div class="card">
            <div class="card-content">
              <p class="card-title-sub">Tempus egestas sed sed risus pretium quam vulputate. Ac feugiat sed lectus</p>
              <p class="substitle">- Kurniawan</p>
            </div>
        </div>
      </div>
      <div class="column">
        <div class="card">
            <div class="card-content">
              <p class="card-title-sub">Tempus egestas sed sed risus pretium quam vulputate. Ac feugiat sed lectus</p>
              <p class="substitle">- Kurniawan</p>
            </div>
        </div>
      </div>
      <div class="column">
        <div class="card">
            <div class="card-content">
              <p class="card-title-sub">Tempus egestas sed sed risus pretium quam vulputate. Ac feugiat sed lectus</p>
              <p class="substitle">- Kurniawan</p>
            </div>
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<script>
import LoremIpsum from 'vue-lorem-ipsum';
export default {
  name: 'home',
  data(){
    return{
      heading:'Soaring to new things',
      subheading:" It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import '../mq'

.card-title
 font-size: 2rem;
 font-weight: 600;
 padding-bottom: 1rem;

.button
  margin-top: 2rem;

.fa-cog
  font-size: 3rem;

.card
 margin-top: 2rem; 

.card-title-sub
 font-size: 1rem;
 font-style: italic;

 .substitle
 font-weight: 500;
 padding: 1rem;  
 
</style>
