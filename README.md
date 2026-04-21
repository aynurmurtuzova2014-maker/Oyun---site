<!DOCTYPE html>
<html>
<head>
<title>Oyun Saytı</title>
</head>
<body style="text-align:center; font-family:sans-serif;">

<h1>🎮 Oyun: Rəqəmi tap</h1>
<p>1-dən 10-a qədər bir rəqəm tutmuşam</p>

<input type="number" id="guess">
<button onclick="yoxla()">Yoxla</button>

<p id="netice"></p>

<script>
let random = Math.floor(Math.random() * 10) + 1;

function yoxla() {
  let guess = document.getElementById("guess").value;
  
  if (guess == random) {
    document.getElementById("netice").innerText = "🎉 Düz tapdın!";
  } else {
    document.getElementById("netice").innerText = "❌ Səhv, yenə yoxla";
  }
}
</script>

</body>
</html>

