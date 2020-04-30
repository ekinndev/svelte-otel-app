<script>
  export let imgSource;
  export let imgAlt;
  export let message;
</script>

<style>
  .testimonial img {
    width: 100px;
    float: left;
    border-radius: 50%;
    margin-right: 20px;
  }
  .testimonial {
    opacity: 0.9;
    padding: 20px;
    border-radius: 5px;
    margin-bottom: 40px;
  }
</style>

<div class="testimonial bg-primary">
  <img src=" {imgSource}" alt={imgAlt} />
  <p>{message}</p>

</div>
