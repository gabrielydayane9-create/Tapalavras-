<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tapalavras Neon</title>

<style>
body {
  margin: 0;
  background: #000;
  color: #fff;
  font-family: Arial, sans-serif;
  text-align: center;
}

h1 {
  font-size: 38px;
  margin-bottom: 10px;
  color: #0ff;
  text-shadow: 0 0 15px #0ff;
}

h2 {
  font-size: 26px;
  margin: 10px 0;
}

.tela {
  display: none;
  padding: 20px;
}

.ativa {
  display: block;
}

input {
  width: 90%;
  padding: 12px;
  margin: 6px 0;
  font-size: 16px;
  border-radius: 8px;
  border: none;
}

button {
  width: 95%;
  padding: 14px;
  margin-top: 15px;
  font-size: 18px;
  border-radius: 10px;
  border: none;
  background: #111;
  color: #0ff;
  box-shadow: 0 0 15px #0ff;
}

.info {
  font-size: 22px;
  margin: 10px 0;
}

.categoria {
  font-size: 30px;
  padding: 15px;
  margin: 15px 0;
  border-radius: 12px;
  box-shadow: 0 0 20px currentColor;
}

.letras {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 10px;
}

.letra {
  padding: 18px;
  font-size: 22px;
  border-radius: 10px;
  background: #111;
  font-weight: bold;
  user-select: none;
  box-shadow: 0 0 10px currentColor;
}

.letra.travada {
  color: #444;
  box-shadow: none;
}

</style>
</head>

<body>

<!-- TELA INICIAL -->
<div class="tela ativa" id="inicio">
  <h1>TAPALAVRAS</h1>
  <h2>Neon Edition</h2>

  <p>Digite os nomes (2 a 5 jogadores)</p>

  <input placeholder="Jogador 1">
  <input placeholder="Jogador 2">
  <input placeholder="Jogador 3">
  <input placeholder="Jogador 4">
  <input placeholder="Jogador 5">

  <button onclick="iniciarJogo()">COMEÇAR</button>
</div>

<!-- TELA DO JOGO -->
<div class="tela" id="jogo">
  <div class="info">
    Jogador atual: <strong id="jogador"></strong><br>
    Tempo: <strong id="tempo">10</strong>s
  </div>

  <div class="categoria" id="categoria"></div>

  <div class="letras" id="letras"></div>
说明
  <button onclick="novaRodada()">Nova rodada</button>
</div>

<script>
const categorias = [
  "Frutas","Cidades","Carro","Objetos","Animais","País",
  "Novelas","Filmes","Cores","Cantor/Cantora",
  "Ator/Atriz","Sobremesas","Profissões","Partes do corpo humano"
];

const coresNeon = ["#0ff","#f0f","#0f0","#ff0","#f00","#09f"];

let jogadores = [];
let jogadorAtual = 0;
let tempo = 10;
let intervalo;
let categoriaAtual = "";

function corNeon() {
  return coresNeon[Math.floor(Math.random()*coresNeon.length)];
}

function iniciarJogo() {
  const inputs = document.querySelectorAll("#inicio input");
  jogadores = [];
  inputs.forEach(i => {
    if (i.value.trim()) jogadores.push(i.value.trim());
  });

  if (jogadores.length < 2) {
    alert("Mínimo 2 jogadores.");
    return;
  }

  document.getElementById("inicio").classList.remove("ativa");
  document.getElementById("jogo").classList.add("ativa");

  novaRodada();
}

function novaRodada() {
  categoriaAtual = categorias[Math.floor(Math.random()*categorias.length)];
  const cor = corNeon();

  document.getElementById("categoria").textContent = categoriaAtual;
  document.getElementById("categoria").style.color = cor;

  jogadorAtual = 0;
  atualizarJogador();

  criarLetras(cor);
}

function atualizarJogador() {
  document.getElementById("jogador").textContent = jogadores[jogadorAtual];
  iniciarTempo();
}

function iniciarTempo() {
  clearInterval(intervalo);
  tempo = 10;
  document.getElementById("tempo").textContent = tempo;

  intervalo = setInterval(() => {
    tempo--;
    document.getElementById("tempo").textContent = tempo;

    if (tempo <= 0) {
      clearInterval(intervalo);
      alert(jogadores[jogadorAtual] + " perdeu a rodada!");
      novaRodada();
    }
  }, 1000);
}

function criarLetras(cor) {
  const letrasDiv = document.getElementById("letras");
  letrasDiv.innerHTML = "";
  const alfabeto = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

  for (let l of alfabeto) {
    const div = document.createElement("div");
    div.className = "letra";
    div.textContent = l;
    div.style.color = cor;

    div.onclick = () => {
      if (div.classList.contains("travada")) return;

      div.classList.add("travada");
      jogadorAtual = (jogadorAtual + 1) % jogadores.length;
      atualizarJogador();
    };

    letrasDiv.appendChild(div);
  }
}
</script>

</body>
</html>
