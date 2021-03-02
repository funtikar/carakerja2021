
<html>
  <head>
    <base target="_top">
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
   
  </head>
  <body>
    <form class="form-horizontal">
<fieldset>

<!-- Form Name -->
<legend>Form Name</legend>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="berat">Berat</label>  
  <div class="col-md-4">
  <input id="berat" name="berat" type="text" placeholder="" class="form-control input-md">
  <span class="help-block">Berat Kamu</span>  
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="tinggi">Tinggi</label>  
  <div class="col-md-4">
  <input id="tinggi" name="tinggi" type="text" placeholder="" class="form-control input-md">
  <span class="help-block">Tinggi kamu</span>  
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="hasil">BMI</label>  
  <div class="col-md-4">
  <input id="hasil" name="hasil" type="text" placeholder="" class="form-control input-md">
  <span class="help-block">BMI kamu!</span>  
  </div>
</div>

</fieldset>
</form>
<script>
  //alert('xss');
const berat = document.getElementById('berat');
const tinggi = document.getElementById('tinggi');
const hasil = document.getElementById('hasil');
berat.addEventListener('input', updateValue);
function updateValue(e) {
  //alert('pronto')
  var gg = berat.value/(tinggi.value/100*tinggi.value/100)
  //alert(gg);
  hasil.value = gg;
}
  </script>

  </body>
</html>
