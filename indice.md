<html>
<TITLE>Ejemplo06.htm</TITLE>

<head>
<script>
//Ejemplo que visualiza un reloj digital.
function Ver_Hora()
{
  var mihora = new Date();
  var horas = mihora.getHours().toString();
  var minutos = mihora.getMinutes().toString();
  if (minutes.length == 1) minutos = "0" + minutos;
  var segundos = mihora.getSeconds().toString();
  if (segundos.length == 1) segundos = "0" + segundos;
  
  document.forms[0].mireloj.value = horas + " : " + minutos + " : " + segundos;
 }
 </script>
 </head>
 <body>
 <form>
 <p align="center">
 <input type="text" size="10" name="mireloj">
 </p>
 </form>
 <script>
  var r = setInterval ("Ver_Hora()",500);
  </script>
  </body>
  
  </html>
