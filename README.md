# AdventCalendar2025
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Ingreso de Código</title>
<style>
  body { font-family: Arial; background:#f2efe4; padding:40px; }
  #box { max-width:400px; margin:auto; background:white; padding:20px; border-radius:10px; }
  input { width:100%; padding:10px; font-size:18px; margin-top:10px; }
  #msg { margin-top:20px; font-size:22px; font-weight:bold; }
</style>
</head>
<body>
<div id="box">
  <h2>Ingresá tu código</h2>
  <input id="code" placeholder="Escribe el código..." oninput="checkCode()" />
  <div id="msg"></div>
</div>

<script>
function checkCode() {
    let c = document.getElementById("code").value.toUpperCase();
    let msg = document.getElementById("msg");

    let respuestas = {
        "LADO": "Perfecto. Avanzaste al siguiente nivel.",
        "AMOR": "La palabra secreta te guía al costado derecho.",
        "219": "¡Código final desbloqueado!"
    };

    msg.innerHTML = respuestas[c] || "";
}
</script>
</body>
</html>
