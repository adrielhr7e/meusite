<style>    
  .codigo-box {    
    text-align: center;    
    margin-top: 20px;    
  }    
    
  /* Animação diferente para o título */    
  @keyframes tituloColorShift {    
    0% { background-position: 0% 50%; }    
    25% { background-position: 50% 50%; }    
    50% { background-position: 100% 50%; }    
    75% { background-position: 50% 50%; }    
    100% { background-position: 0% 50%; }    
  }    
    
  .titulo-animado {    
    display: inline-block;    
    padding: 10px 20px;    
    border-radius: 10px;    
    border: 2px solid transparent;    
    background: linear-gradient(45deg, #FF4500, #FFD700, #FF69B4, #1E90FF); /* cores quentes e frias misturadas */    
    background-size: 300% 300%;    
    animation: tituloColorShift 5s ease infinite;    
    color: white;    
    font-weight: bold;    
    font-size: 16px;    
    text-transform: uppercase;    
    margin-bottom: 20px;    
    position: relative;    
  }    
    
  .titulo-animado::before {    
    content: "";    
    position: absolute;    
    top: -2px; bottom: -2px; left: -2px; right: -2px;    
    border-radius: 12px;    
    background: linear-gradient(45deg, #FF4500, #FFD700, #FF69B4, #1E90FF);    
    background-size: 300% 300%;    
    animation: tituloColorShift 5s ease infinite;    
    z-index: -1;    
  }    
    
  /* restante do código permanece igual */    
    
  .copiar-container {    
    position: relative;    
    border: 2px solid #000;    
    border-radius: 10px;    
    padding: 20px 14px;    
    margin: 12px auto;    
    width: 320px;    
    background-color: #111;    
    color: white;    
    font-size: 14px;    
  }    
    
  .botao-copiar {    
    padding: 6px 10px;    
    font-size: 14px;    
    font-weight: bold;    
    border: none;    
    border-radius: 8px;    
    cursor: pointer;    
    width: 100%;    
    color: white;    
    text-transform: uppercase;    
    background: linear-gradient(45deg, purple, red, orange, green);    
    background-size: 400% 400%;    
    animation: colorShift 6s ease infinite;    
  }    
    
  @keyframes colorShift {    
    0% { background-position: 0% 50% }    
    50% { background-position: 100% 50% }    
    100% { background-position: 0% 50% }    
  }    
    
  .mensagem {    
    font-weight: bold;    
    padding: 8px;    
    margin-top: 10px;    
    border-radius: 6px;    
    font-size: 14px;    
    display: none;    
    text-transform: lowercase;    
    animation: colorShift 6s ease infinite;    
  }   
   #container1 .mensagem {    
    color: #4a90e2;    
    background-color: #152a4d;    
  }    
  #container2 .mensagem {    
    color: #4caf50;    
    background-color: #1b3a1b;    
  }    
  #container3 .mensagem {    
    color: #f57c00;    
    background-color: #4e2e00;    
  }    
    
  .abrir-ff {    
    background-color: #444;    
    padding: 6px 8px;    
    font-size: 12px;    
    color: white;    
    border: none;    
    border-radius: 6px;    
    cursor: pointer;    
    margin-top: 6px;    
    width: 320px;    
    display: none;    
    margin-left: auto;    
    margin-right: auto;    
    text-transform: lowercase;    
  }    
    
  /* Botões TikTok e E-mail estilizados iguais */    
  .botao-tiktok, .botao-email {    
    margin-top: 30px;    
    padding: 6px 10px;    
    font-size: 14px;    
    font-weight: bold;    
    border: none;    
    border-radius: 10px;    
    cursor: pointer;    
    width: 160px;    
    color: white;    
    text-transform: none;    
    background: linear-gradient(45deg, red, blue, cyan, magenta);    
    background-size: 400% 400%;    
    animation: colorShift 6s ease infinite;    
    display: flex;    
    
    align-items: center;    
    justify-content: center;    
    gap: 8px;    
  }    
    
  .botao-tiktok svg, .botao-email svg {    
    width: 20px;    
    height: 20px;    
    fill: white;    
  }    
    
  /* Container para botões lado a lado */    
  .botoes-lado-a-lado {    
    display: flex;    
    justify-content: center;    
    gap: 16px;    
    margin-top: 30px;    
  }    
</style>  <div class="codigo-box">      <div class="titulo-animado">CÓDIGO DO MAPA TERRENO LIVRE</div>    <div class="copiar-container" id="container1">    <button class="botao-copiar" onclick="copiarCodigo('#FREEFIRE8D61E9C78D2369027CE28FB442566BA38304', 'container1', this)">COPIAR CÓDIGO TERRENO LIVRE 4X4</button>    
<div class="mensagem"></div>    
<button class="abrir-ff" onclick="abrirFreeFire()">abrir jogo — o aplicativo será iniciado automaticamente</button>

  </div>    <div class="copiar-container" id="container2">    
    <button class="botao-copiar" onclick="copiarCodigo('#FREEFIREDBB16BB2D16950ADADCDD3DC3C5C531D8304', 'container2', this)">COPIAR CÓDIGO TERRENO LIVRE 2X2</button>    
     <div class="mensagem"></div>    
    <button class="abrir-ff" onclick="abrirFreeFire()">abrir jogo — o aplicativo será iniciado automaticamente</button>    
  </div>    <div class="copiar-container" id="container3">    
    <button class="botao-copiar" onclick="copiarCodigo('#FREEFIRE96E89A45A61545EE43CD478F954E26928304', 'container3', this)">COPIAR CÓDIGO TERRENO LIVRE 1X1</button>    
    <div class="mensagem"></div>    
    <button class="abrir-ff" onclick="abrirFreeFire()">abrir jogo — o aplicativo será iniciado automaticamente</button>    
  </div>    <!--Botões TikTok e E-mail lado a lado-->    <div class="botoes-lado-a-lado">    
    <button class="botao-tiktok" onclick="abrirTikTok()">    
      <svg aria-hidden="true" focusable="false" viewbox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">    
        <path d="M9.94 2.5v15.15a4.48 4.48 0 1 1-3.19-4.23v-4.6a8.86 8.86 0 0 0 3.19.28z">    
        <path d="M15.5 8.43a5.23 5.23 0 0 1-2.65-.69v6.2a4.48 4.48 0 1 1-3.19-4.23v-9.7h2.92v6.92a8.72 8.72 0 0 0 3.6 1.5z">    
      </path></path></svg>    
      Tik Tok    
    </button>  <button class="botao-email" onclick="abrirEmail()">    
  <svg fill="white" height="20px" viewbox="0 0 24 24" width="20px" xmlns="http://www.w3.org/2000/svg">    
    <path d="M0 4a2 2 0 0 1 2-2h20a2 2 0 0 1 2 2v16a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V4zm2 0v.511L12 13l10-8.489V4H2zm20 16V8.199L14.803 15 22 20zm-2 0l-7-6-7 6h14zm-18 0v-1.801L9.197 15 2 8.2V20z">    
  </path></svg>    E-mail    
</button>    </div>    
</div>  <script>    
function copiarCodigo(codigo, idAtivo, botao) {    
  const containers = document.querySelectorAll('.copiar-container');    
  containers.forEach(container => {    
    const msg = container.querySelector('.mensagem');    
    const abrirBtn = container.querySelector('.abrir-ff');    
    const botaoCopiar = container.querySelector('.botao-copiar');    
    msg.style.display = "none";    
    msg.innerHTML = "";    
    abrirBtn.style.display = "none";    
    botaoCopiar.style.display = "inline-block";    
  });    const tempInput = document.createElement("input");
document.body.appendChild(tempInput);
tempInput.value = codigo;
tempInput.select();
document.execCommand("copy");
document.body.removeChild(tempInput);const ativo = document.getElementById(idAtivo); const msgAtivo = ativo.querySelector('.mensagem'); const abrirBtnAtivo = ativo.querySelector('.abrir-ff'); const botaoCopiarAtivo = ativo.querySelector('.botao-copiar');

msgAtivo.textContent = "código copiado com sucesso!"; msgAtivo.style.display = "block"; abrirBtnAtivo.style.display = "block";

botaoCopiarAtivo.style.display = "none"; }

function abrirFreeFire() { window.location.href = "freefire://"; }

function abrirTikTok() { window.location.href = "snssdk1128://"; setTimeout(() => { window.open("https://www.tiktok.com/@m_moreno_35", "_blank"); }, 1500); }

function abrirEmail() { window.location.href = "mailto:adrieltorresoliveira123@gmail.com"; }

</script>
