<script>
  export let baslik;
  export let metin;
  export let bgColor;
  export let fontIcon;
  export let size;
</script>

<style>
  .box {
    float: left;
    width: 33.3%;
    padding: 50px;
    text-align: center;
  }

  .box i {
    margin-bottom: 10px;
  }
  @media screen and (max-width: 768px) {
    .box {
      float: none;
      width: 100%;
    }
    
  }
</style>

<div class="box {bgColor}">
  <i class="{fontIcon} {size}" />

  <h3>{baslik}</h3>
  <p>{metin}</p>
</div>
