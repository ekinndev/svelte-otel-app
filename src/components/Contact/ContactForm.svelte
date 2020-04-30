<script>
  import Button from "../../UI/Button.svelte";
  import Input from "../../UI/Input.svelte";
</script>

<section id="contact-form" class="py-3">
  <div class="container">
    <h1 class="l-heading">
      <span class="text-primary">İletişime</span>
      Geç
    </h1>
    <p>
      Aşağıdaki formu doldurarak bizimle iletişime geçebilirsiniz.Size en kısa
      zamanda döneceğiz.
    </p>
    <form action="" method="POST">

      <Input type="text" idName="name" isim="İsim" />

      <Input type="email" idName="email" isim="Email" />

      <Input type="textarea" idName="message" isim="Mesaj" />

      <Button type="submit">Submit</Button>
    </form>

  </div>
</section>
