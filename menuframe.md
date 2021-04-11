<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<body>

<div class="w3-sidebar w3-bar-block w3-black w3-card" style="width:150px">
  <h5 class="w3-bar-item">Novidades</h5>
  <button class="w3-bar-item w3-button tablink" onclick="openLink(event, 'Left1')">Comercial</button>
  <button class="w3-bar-item w3-button tablink" onclick="openLink(event, 'Left2')">Ética</button>
  <button class="w3-bar-item w3-button tablink" onclick="openLink(event, 'Left3')">Legislação</button>
</div>

<div style="margin-left:150px">
  <div class="w3-padding">Atualização</div>

  <div id="Left1" class="w3-container city w3-animate-left" style="display:none">
    <h2>Comercial</h2>
<ul>
  <li>Exercícios de DEMONSTRAÇÃO DOS LUCROS OU PREJUÍZOS ACUMULADOS adicionados; </li>
</ul>
  </div>

  <div id="Left2" class="w3-container city w3-animate-left" style="display:none">
    <h2>Ética</h2>
<ul>
  <li>Conteúdo ainda no AVA; </li>
</ul>
  </div>

  <div id="Left3" class="w3-container city w3-animate-left" style="display:none">
    <h2>Legislação</h2>
<ul>
  <li>Aula 9 disponível; </li>
</ul>
  </div>

</div>

<script>
function openLink(evt, animName) {
  var i, x, tablinks;
  x = document.getElementsByClassName("city");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < x.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" w3-red", "");
  }
  document.getElementById(animName).style.display = "block";
  evt.currentTarget.className += " w3-red";
}
</script>

</body>
</html>