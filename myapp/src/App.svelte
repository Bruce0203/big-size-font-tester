<link rel="stylesheet" href="https://unpkg.com/@picocss/pico@latest/css/pico.min.css">

<strong id="text">text</strong>
<form>
  <input type="text" id="text" name="text" placeholder="text" required>
</form>
<style>
  form {
    position: absolute;
  bottom: 0px;
  }
</style>
<script>
const input = document.querySelector('input');
const log = document.getElementById('text');

input.addEventListener('input', updateValue);

function updateValue(e) {
  log.textContent = e.target.value;
}

</script>