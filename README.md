<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ciclo da Borracha - Aprendizado Divertido</title>
<style>
body {font-family: Arial, sans-serif; background: linear-gradient(180deg, #d0f0c0, #a0e0ff); margin: 0; padding: 0; text-align: center;}
header {background-color: #228b22; color: white; padding: 20px 10px;}
main {padding: 20px;}
.card {background-color: white; margin: 10px auto; padding: 15px; border-radius: 10px; width: 90%; max-width: 600px; box-shadow: 0 2px 6px rgba(0,0,0,0.2);}
button {background-color: #228b22; color: white; border: none; padding: 10px 15px; border-radius: 5px; cursor: pointer; margin-top: 10px;}
button:hover {background-color: #1a661a;}
.hidden {display: none;}
.feedback {margin-top: 10px; font-weight: bold;}
footer {background-color: #f0f0f0; padding: 20px; font-size: 14px; margin-top: 30px;}
footer a {color: #006400; text-decoration: none;}
footer a:hover {text-decoration: underline;}
</style>
</head>
<body>
<header>
<h1>O Ciclo da Borracha</h1>
<p>Descubra como a borracha mudou o Brasil!</p>
</header>
<main>

<div id="etapa1" class="card">
<h2>1. O Início: o Seringal</h2>
<p>No meio da floresta amazônica, os seringueiros extraíam o látex das seringueiras, um líquido branco que é a base da borracha.</p>
<button onclick="mostrar('etapa2')">Próxima etapa</button>
</div>

<div id="etapa2" class="card hidden">
<h2>2. A Coagulação</h2>
<p>O látex era tratado com produtos químicos, formando uma massa sólida. Depois era prensado em folhas e deixado para secar.</p>
<button onclick="mostrar('etapa3')">Próxima etapa</button>
</div>

<div id="etapa3" class="card hidden">
<h2>3. A Industrialização</h2>
<p>Com a borracha seca, as fábricas produziam pneus, luvas e muitos outros produtos. O auge foi entre 1890 e 1920!</p>
<button onclick="mostrar('etapa4')">Próxima etapa</button>
</div>

<div id="etapa4" class="card hidden">
<h2>4. Impacto Social</h2>
<p>Durante o auge do ciclo, milhares de trabalhadores nordestinos migraram para a Amazônia em busca de trabalho nos seringais, enfrentando condições difíceis e vida isolada na floresta.</p>
<button onclick="mostrar('curiosidades')">Ver curiosidades</button>
</div>

<div id="curiosidades" class="card hidden">
<h2>Curiosidades!</h2>
<ul style="text-align:left;max-width:500px;margin:auto;">
<li>Manaus ficou riquíssima com o comércio da borracha.</li>
<li>O Teatro Amazonas foi construído nessa época.</li>
<li>O ciclo acabou quando os ingleses começaram a plantar seringueiras na Ásia.</li>
<li>A borracha foi fundamental para a Revolução Industrial e para a fabricação de pneus no mundo todo.</li>
</ul>
<button onclick="mostrar('quiz1')">Realizar um Quiz!</button>
</div>

<!-- Quiz 1 -->
<div id="quiz1" class="card hidden">
<h2>Quiz 1</h2>
<p>Onde nasceu o Ciclo da Borracha?</p>
<div>
<button onclick="responder('quiz1', true, 'quiz2')">Na Amazônia</button>
<button onclick="responder('quiz1', false, 'quiz2')">Na Europa</button>
</div>
<p id="quiz1-feedback" class="feedback"></p>
</div>

<!-- Quiz 2 -->
<div id="quiz2" class="card hidden">
<h2>Quiz 2</h2>
<p>Qual cidade ficou famosa por causa do ciclo da borracha?</p>
<div>
<button onclick="responder('quiz2', true, 'quiz3')">Manaus</button>
<button onclick="responder('quiz2', false, 'quiz3')">São Paulo</button>
</div>
<p id="quiz2-feedback" class="feedback"></p>
</div>

<!-- Quiz 3 -->
<div id="quiz3" class="card hidden">
<h2>Quiz 3</h2>
<p>O que é extraído da seringueira?</p>
<div>
<button onclick="responder('quiz3', true, 'quiz4')">Látex</button>
<button onclick="responder('quiz3', false, 'quiz4')">Petróleo</button>
</div>
<p id="quiz3-feedback" class="feedback"></p>
</div>

<!-- Quiz 4 -->
<div id="quiz4" class="card hidden">
<h2>Quiz 4</h2>
<p>Por que o Ciclo da Borracha acabou?</p>
<div>
<button onclick="responder('quiz4', true, 'quiz5')">Porque a produção passou para a Ásia</button>
<button onclick="responder('quiz4', false, 'quiz5')">Porque acabou o látex no Brasil</button>
</div>
<p id="quiz4-feedback" class="feedback"></p>
</div>

<!-- Quiz 5 -->
<div id="quiz5" class="card hidden">
<h2>Quiz 5</h2>
<p>Qual foi um dos principais impactos sociais do Ciclo da Borracha?</p>
<div>
<button onclick="responder('quiz5', true, 'final')">Migração de trabalhadores nordestinos para a Amazônia</button>
<button onclick="responder('quiz5', false, 'final')">Fim da industrialização em Manaus</button>
</div>
<p id="quiz5-feedback" class="feedback"></p>
</div>

<div id="final" class="card hidden">
<h2>Parabéns!</h2>
<p>Você concluiu o aprendizado sobre o Ciclo da Borracha! 🌿</p>
<p>Agora você sabe como a Amazônia viveu um dos períodos mais marcantes da história econômica do Brasil.</p>
</div>
</main>

<footer>
<h3>Fontes de Pesquisa</h3>
<ul style="list-style:none; padding:0;">
<li><a href="https://brasilescola.uol.com.br/historiab/ciclo-borracha.htm" target="_blank">Brasil Escola - Ciclo da Borracha</a></li>
<li><a href="https://mundoeducacao.uol.com.br/historiadobrasil/ciclo-da-borracha.htm" target="_blank">Mundo Educação - Ciclo da Borracha</a></li>
<li><a href="https://www.todamateria.com.br/ciclo-da-borracha/" target="_blank">Toda Matéria - Ciclo da Borracha</a></li>
<li><a href="https://www.politize.com.br/exploracao-de-borracha-na-amazonia/" target="_blank">Politize! - Exploração da Borracha na Amazônia</a></li>
</ul>
</footer>

<script>
function mostrar(id){
  document.getElementById(id).classList.remove('hidden');
  window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' });
}
function responder(quizId, correta, proximoId){
  const feedback = document.getElementById(quizId + '-feedback');
  feedback.textContent = correta ? '🎉 Correto!' : '❌ Errado!';
  feedback.style.color = correta ? 'green' : 'red';
  const quizDiv = document.getElementById(quizId);
  const buttons = quizDiv.querySelectorAll('div button');
  buttons.forEach(b => b.disabled = true);
  setTimeout(()=>{mostrar(proximoId)}, 800);
}
</script>
</body>
</html>

