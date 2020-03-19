<template>
<html>

<body>
    <div class="my-jumbotron" id="my-jumbotron">
      <nav class="navbar navbar-expand">
        <img src="./pictures/rueve-logo.svg" class="navbar-brand p-2"/>
        <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="" >Home</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">About</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Shop</a>
        </li>
        </ul>
        <div class="collapse navbar-collapse">
          <ul class="nav navbar-nav ml-auto">
          <li class="nav-item mx-3  ">
              <a class="nav-link" href=""><img src="./pictures/user.svg" width="30px" height="30px"/></a>
          </li>
          <li class="nav-item mx-2">
              <a class="nav-link" href=""><img src="./pictures/shopping-cart.svg" width="30px" height="30px"/></a>
          </li>
          </ul>
        </div>
        </nav>
  <div class="container-fluid">
  <div id="myCarousel" class="carousel slide" data-ride="carousel">
  <!-- Indicators -->
  <!-- <ol class="carousel-indicators">
    <li data-target="#myCarousel" data-slide-to="0" class="active"></li>
    <li data-target="#myCarousel" data-slide-to="1"></li>
    <li data-target="#myCarousel" data-slide-to="2"></li>
  </ol> -->

  <!-- Wrapper for slides -->
  <div class="carousel-inner">
    <div class="item active">
      <img src="./pictures/1.jpg" alt="Retail" style="width:100%;">
    </div>

    <div class="item">
      <img src="./pictures/2.jpeg" alt="Yezzy" style="width:100%;">
    </div>

    <div class="item">
      <img src="./pictures/3.jpeg" alt="Nike" style="width:100%;">
    </div>
  </div>

  <!-- Left and right controls -->
  <a class="left carousel-control" href="#myC arousel" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" href="#myCarousel" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
</div>
        <div class="container text-center" id="jumbo-text-contain">
            <h3 class="display-4 mt-5">Welcome To Footwear Store </h3>
            <h4 class="lead">Trusted Sneakers Marketplace</h4>
            <button type="button" class="btn" id="jumbotron-btn">SHOP NOW !</button>
        </div>
    </div>
<div id="category-sect">
    <h1 class="font-weight-bold pt-5 text-center">SNEAKERS</h1>
      <section id="tabs" class="project-tab">
        <div class="container-fluid">
            <div class="row justify-content-center">
                <div class="col-md-12">
                    <b-tabs content-class="mt-3" fill>
                    <b-tab title="Converse" active>
                    <ul class="container mt-4">
                          <div class="row">
                        <div v-for="(converse, index) in converses" :key="index" class="my-3 mr-2 text-center">
                          <div class="product-image">
                               <img src="./pictures/Converse1.jpg" class="img-responsive h-75 w-100 p-2"/>
                               <!-- <img :src="/pictures/ + fileconverse + index + filetype" class="img-responsive h-75 w-100 p-2"/> -->
                            </div>
                          <div class="product-details">
                            <h6 class="display-6 mt-3">{{ converse.name }}</h6>
                            <h6 class="display-6 text-muted">Rp.{{ converse.price }}</h6>
                          </div>
                        </div>
                    </div>
                    </ul>
                    </b-tab>
                    <b-tab title="Adidas">
                      <ul class="container mt-4">
                          <div class="row">
                        <div v-for="( adidas, index) in adidass" :key="index" class="my-3 mr-2 text-center">
                          <div class="product-image">
                            <img src="./pictures/Adidas1.jpg" class="img-responsive h-75 w-100 p-2"/>
                            <!-- <img :src="/pictures/ + fileadidas + index + filetype" class="img-responsive h-75 w-100 p-2"/> -->
                            </div>
                          <div class="product-details">
                            <h6 class="display-6 mt-3">{{ adidas.name }}</h6>
                            <h6 class="display-6 text-muted">Rp.{{ adidas.price }}</h6>
                          </div>
                        </div>
                    </div>
                    </ul>
                      </b-tab>
                      <b-tab title="Nike">
                      <ul class="container mt-4">
                          <div class="row">
                        <div v-for="(nike, index) in nikes" :key="index" class="my-3 mr-2 text-center">
                          <div class="product-image">
                            <img src="./pictures/Nike1.jpg" class="img-responsive h-75 w-100 p-2"/>
                            <!-- <img :src="/pictures/ + filenike + index + filetype" class="img-responsive h-75 w-100 p-2"/> -->
                            </div>
                          <div class="product-details">
                            <h6 class="display-6 mt-3">{{ nike.name }}</h6>
                            <h6 class="display-6 text-muted">Rp.{{ nike.price }}</h6>
                          </div>
                        </div>
                    </div>
                    </ul>
                    </b-tab>
                  </b-tabs>

                    </div>
                </div>
            </div>
            </section>
        </div>
</body>
<footer class="page-footer blue pt-5 mt-5">
<div class="container-fluid text-center text-md-left">
      <div class="row">
        <div class="col-md-6 mt-md-0 mt-3">
          <img class="px-5" src="./pictures/rueve-logo.svg" />
          <p class="text-md-left px-5">Footwear Store berusaha menciptakan marketplace yang aman dan efisien bagi pembeli dan penjual sneakers untuk melakukan transaksi.</p>

        </div>

        <hr class="clearfix w-100 d-md-none pb-3">
        <div class="col-md-3 mb-md-0 mb-3">

          <h5 class="text-uppercase">FAQ</h5>

          <ul class="list-unstyled">
            <li>
              <a href="#!">Panduan Pembayaran</a>
            </li>
            <li>
              <a href="#!">FAQ</a>
            </li>
            <li>
              <a href="#!">Terms & Conditions</a>
            </li>
            <li>
              <a href="#!">Privacy Policy</a>
            </li>
          </ul>

        </div>
        <div class="col-md-3 mb-md-0 mb-3">

          <h5 class="text-uppercase">Contact</h5>

          <ul class="list-unstyled">
            <li>
              <a href="#!">Instagram</a>
            </li>
            <li>
              <a href="#!">Whatsapp</a>
            </li>
            <li>
              <a href="#!">Line</a>
            </li>
            <li>
              <a href="#!">G mail</a>
            </li>
          </ul>

        </div>

      </div>

    </div>

    <div class="footer-copyright text-right py-3 mr-3">© 2020 Copyright: Footwear
    </div>
  </footer>

</html>
  <!-- <div id="app">
    <h1 v-for="(converse, index) in converses" :key="index">{{ converse.name }}</h1>
    <h1 v-for="(tconverse, index) in tconverses" :key="index">{{ adidasprice }}</h1>
    </div> -->
</template>

<script>
import axios from 'axios'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

export default {
  name: 'App',
  data () {
    return {
      // filetype: '.jpg',
      // fileconverse: 'converse',
      // fileadidas: 'adidas',
      // filenike: 'nike',
      adidass: [],
      converses: [],
      nikes: []
    }
  },
  async created () {
    const baseURI = 'https://my-json-server.typicode.com/BayuNova/ftwr1/db'
    axios.get(baseURI)
      .then((result) => {
        this.adidass = result.data.adidass
        this.converses = result.data.converses
        this.nikes = result.data.nikes
      })
  }
}

</script>

<style>
#my-jumbotron {
    background-color: #cccccc;
    background-size: cover;
    overflow: hidden;
}
#jumbo-text-contain {
    color: black;
    min-height: 400px;
}
#jumbotron-btn {
    font-size: 50px;
    border: 3px solid ;
    border-radius: 0;
    transition: 0.3s;
}
#jumbotron-btn:hover {
    color:white ;
    border: 1px solid white;
}
#products-container li{
    list-style-type: none;
    height: 250px;
}
.product-image {
    background: #f4f4ef;
    width: 250px;
    height: 275px;
}
.project-tab {
    padding: 10%;
    margin-top: -8%;
}
.project-tab #tabs{
    background: #007b5e;
    color: #eee;
}
.project-tab #tabs h6.section-title{
    color: #eee;
}
.project-tab #tabs .nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link.active {
    color: #20232a;
    background-color: transparent;
    border-color: transparent transparent #f3f3f3;
    border-bottom: 3px solid !important;
    font-size: 20px;
    font-weight: bold;
}
.project-tab .nav-link {
    border: 1px solid transparent;
    border-top-left-radius: .25rem;
    border-top-right-radius: .25rem;
    color: #acbebe;
    font-size: 20px;
    font-weight: 600;
}
.project-tab .nav-link:hover {
    border: none;
}
.project-tab thead{
    background: #f3f3f3;
    color: #333;
}
.project-tab a{
    text-decoration: none;
    color: #333;
    font-weight: 600;
}
.page-footer {
    color: black;
    background: #cccccc;
}
</style>
