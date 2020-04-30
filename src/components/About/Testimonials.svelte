<script>
  import Testimonial from "../../UI/Testimonial.svelte";
</script>

<style>
  #testimonials h2 {
    color: white;
    text-align: center;
    text-align: center;
    padding-bottom: 40px;
  }
  #testimonials {
    height: 100%px;
    background: url("../img/test-bg.jpg") no-repeat center center/cover;
    padding-top: 100px;
  }
</style>

<section id="testimonials" class="py-3">
  <div class="container">
    <h2 class="l-heading">Misafirlerimiz ne Söyledi ?</h2>

    <Testimonial
      imgSource="./img/person-1.jpg"
      imgAlt="Samantha"
      message="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos
      quam hic at culpa ipsam. Magnam dolorem qui repellat aliquid ratione
      molestiae error quo, sequi a mollitia earum, iusto repudiandae, quam
      commodi. Ducimus hic alias impedit eum id, quam velit dicta." />

    <Testimonial
      imgSource="./img/person-2.jpg"
      imgAlt="Jean"
      message="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos
      quam hic at culpa ipsam. Magnam dolorem qui repellat aliquid ratione
      molestiae error quo, sequi a mollitia earum, iusto repudiandae, quam
      commodi. Ducimus hic alias impedit eum id, quam velit dicta." />

  </div>

</section>
