<style>
  #about-info .info-right {
    float: right;
    width: 50%;
    min-height: 100%;
  }
  #about-info .info-right img {
    width: 70%;
    margin: auto;
    display: block;
    border-radius: 50%;
  }
  #about-info .info-left {
    float: left;
    width: 50%;
    min-height: 100%;
  }
  @media screen and (max-width: 768px) {
    #about-info .info-right,
    #about-info .info-left {
      float: none;
      width: 100%;
    }
    #about-info .info-right {
      margin-top: 30px;
    }
  }
</style>

<section id="about-info" class="bg-light py-3">
  <div class="container">
    <div class="info-left">

      <h1 class="l-heading">
        Svelte Otel
        <span class="text-primary">Hakkında</span>
      </h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae impedit
        quisquam adipisci consequatur minus totam ipsa delectus similique! Alias
        similique totam facilis quam impedit veniam iste maxime in laboriosam
        esse!
      </p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis porro
        inventore molestias quis eligendi tempore odio veniam est quasi
        exercitationem.
      </p>

    </div>
    <div class="info-right">
      <img src="./img/photo-2.jpg" alt="hotel" />
    </div>
  </div>
</section>
<div class="clr" />
