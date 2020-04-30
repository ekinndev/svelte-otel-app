<script>
  export let idName;
  export let isim;
  export let type = "text";
</script>

<style>
  .form-group {
    margin-bottom: 20px;
  }
  label {
    display: block;
    margin-bottom: 5px;
  }
  input,
  textarea {
    width: 100%;
    padding: 10px;
    border: 1px #ddd solid;
  }
  textarea {
    height: 200px;
  }
  input:focus,
  textarea:focus {
    outline: none;
    border-color: #f7c08a;
  }
</style>

<div class="form-group">
  <label for={idName}>{isim}</label>
  {#if type === 'textarea'}
    <textarea name={idName} id={idName} />
  {:else}
    <input {type} name={idName} id={idName} />
  {/if}
</div>
