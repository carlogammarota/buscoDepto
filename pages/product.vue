<template>

        <div class="columns is-full">
          <!--<div class="column is-4">-->
            <!--First column-->
          <!--</div>-->

          <div class="column is-4" v-for="(item, index) in products">
            <div class="card">
              <div class="card-image">
                <figure class="image is-4by3">
                  <img :src="item.img" alt="Placeholder image">
                </figure>
              </div>
              <div class="card-content">
                <!--<div class="media">-->
                  <!--<div class="media-left">-->
                    <!--<figure class="image is-48x48">-->
                      <!--<img src="https://bulma.io/images/placeholders/96x96.png" alt="Placeholder image">-->
                    <!--</figure>-->
                  <!--</div>-->
                  <!--<div class="media-content">-->
                    <!--<p class="title is-4">John Smith</p>-->
                    <!--<p class="subtitle is-6">@johnsmith</p>-->
                  <!--</div>-->
                <!--</div>-->

                <h3 class="price">${{item.price}} /Per Month</h3>

                <div class="content">
                  <p class="des">{{item.des}}</p>
                  <p class="address"><fa :icon="['fas', 'dollar-sign']" /> {{item.address}}</p>


                  <br>
                  <div class="columns info">
                    <div class="column is-3">
                      <fa :icon="['fas', 'dollar-sign']" /> Beds: {{item.Beds}}

                    </div>
                    <div class="column is-3">
                      <fa :icon="['fas', 'dollar-sign']" /> Baths: {{item.Baths}}
                    </div>
                    <div class="column">
                      <fa :icon="['fas', 'dollar-sign']" /> Area: {{item.Area}}
                    </div>
                  </div>
                  <a>@{{item.author}}</a>
                  <a href="#">#casa</a> <a href="#">#pileta</a>
                  <time datetime="2017-1-1">11:09 PM - 1 Jan 2016</time>
                </div>
              </div>
            </div>
          </div>
          <!--<div class="column is-4 is-0color">-->
            <!--Third column-->
            <!--<fa :icon="['fas', 'dollar-sign']" />-->
          <!--</div>-->
        </div>

</template>

<script>
    export default {
        name: "product",
        data(){
          return {
            products: [
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
              {author: "Carlo Gammarota", img:"http://www.nordestenoticias.com.ar/wp-content/uploads/2018/08/01-4.jpg", price: 10000, des:"House in Kent Street", address:"127 Kent Street, Sydny, NEW 2000", Beds:3, Baths:2, Area:"587 sq ft"},
            ]
            }
          }
    }
</script>

<style scoped>
  .info{
    font-size: 15px;
  }
  .price{
    color: dodgerblue;
    font-size: 25px;
  }
  .des{
    font-size: 15px;

  }
  .address{
    font-size: 13px;
    color: #7f828b;

  }
</style>
