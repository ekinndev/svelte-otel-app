<script>
  import Button from "../../UI/Button.svelte";
</script>

<style>
  #home-info {
    height: 450px;
  }
  #home-info .info-img {
    float: left;
    width: 50%;
    background: url("../img/photo-1.jpg") no-repeat;
    min-height: 100%;
  }
  #home-info .info-content {
    float: right;
    width: 50%;
    min-height: 100%;
    text-align: center;
    padding: 50px 30px;
    overflow: hidden;
  }
  #home-info .info-content p {
    padding-bottom: 30px;
  }
  @media screen and (max-width: 768px) {
    #home-info {
      height: 550px;
    }
    #home-info .info-img {
      display: none;
    }
    #home-info .info-content {
      float: none;
      width: 100%;
      overflow: hidden;
    }
  }
</style>

<section id="home-info" class="bg-dark">
  <div class="info-img" />
  <div class="info-content">
    <h2>
      Otelimizin
      <span class="text-primary">Tarihi</span>

    </h2>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eius adipisci
      error, illum nemo fuga doloremque fugiat at odit architecto laudantium
      porro eveniet aliquam quia dolorum animi ipsam laborum sequi consequatur,
      unde excepturi explicabo tenetur nihil! Deleniti ea et eius culpa.
    </p>
    <Button href="hakkimizda" lightOrDark={true}>Devamını Oku</Button>
  </div>
</section>
