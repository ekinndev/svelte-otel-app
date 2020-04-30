<script>
  import Button from "../../UI/Button.svelte";
</script>

<style>
  /*Showcase*/
  #showcase {
    background: url("../img/showcase.jpg") no-repeat center center/cover;
    background-position: center center;
    background-repeat: cover;
    height: 600px;
  }

  #showcase .showcase-content {
    color: #fff;
    text-align: center;
    padding-top: 170px;
  }
  #showcase .showcase-content h1 {
    font-size: 60px;
    line-height: 1.2em;
  }
  #showcase .showcase-content p {
    padding-bottom: 20px;
    line-height: 1.7em;
  }
</style>

<div id="showcase">
  <div class="container">
    <div class="showcase-content">
      <h1>
        <span class="text-primary">İyi</span>
        Eğlenceler
      </h1>
      <p class="lead">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero,
        veritatis dignissimos. Libero excepturi omnis voluptatibus?
      </p>
      <Button href="hakkimizda">Hakkımızda</Button>
    </div>
  </div>

</div>
