<!DOCTYPE html>
<html lang="pt-BR">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora rafinha</title>
    <link rel="stylesheet" href="css/menu.css">
    <link rel="stylesheet" href="css/calculadora.css">
    <link rel="stylesheet" href="css/equacaoEntredoisPontos.css">
</head>

<body>

    <nav>
        <a href="index.html">Clássica</a>
        <a href="equaçaoEntreDoisPontos.html" class="selecionada">Equação entre Dois Pontos</a>
        <a href="distanciaEntrePontoeReta.html">Distância entre Ponto e Reta</a>
        <a href="equaçaoReduzida.html">Equação Reduzida</a>
        <a href="posiçaoRelativadasRetas.html">Posição Relativa das Retas</a>
    </nav>

    <div class="calculadora">
        <input type="text" disabled class="display" id="display">

        <div class="pontos">
            <label> Ponto A</label>
            <div><span>X:</span><input type="number" class="ponto" id="xPontoA"></div>
            <div><span>Y:</span><input type="number" class="ponto" id="yPontoA"></div>
        </div>
        <div class="pontos">
            <label> Ponto B</label>
            <div><span>X:</span><input type="number" class="ponto" id="xPontoB"></div>
            <div><span>Y:</span><input type="number" class="ponto" id="yPontoB"></div>
        </div>

    <div class="primeira-linha">
        <button onclick="limpar()">LIMPAR</button>
    </div> 

    <div class="botoes-calculo">
        <button onclick="calcularDistancia()">Distância</button>
        <button onclick="calcularPontoMedio()">Ponto Médio</button>
        <button onclick="calcularEquacaoReta()">Equação da Reta</button>
        <button onclick="calcularCoeficiente()">Coêficiente</button>
    </div>
</div>

    <script src="javascript/equecaodoispontos.js"></script>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora rafinha</title>
    <link rel="stylesheet" href="css/menu.css">
    <link rel="stylesheet" href="css/calculadora.css">
    <link rel="stylesheet" href="css/equacaoReduzida.css">

</head>
<body>

<nav>
    <a href="index.html">Clássica</a>
    <a href="equaçaoEntreDoisPontos.html">Equação entre Dois Pontos</a>
    <a href="distanciaEntrePontoeReta.html">Distância entre Ponto e Reta</a>
    <a href="equaçaoReduzida.html" class="selecionada">Equação Reduzida</a>
    <a href="posiçaoRelativadasRetas.html">Posição Relativa das Retas</a>

</nav>

<div class="calculadora">
    <input type="text" disabled class="display" id="display">

    <div class="pontos">
        <label> Ponto A</label>
        <div><span>X:</span><input type="number" class="ponto" id="x"></div>
        <div><span>Y:</span><input type="number" class="ponto" id="y"></div>
    </div>

    <div class="equacao">
       
        <div><span>Coêficiente Angular</span><input type="number" class="ponto" id="coefieciente"></div>
    </div>

    <div class="primeira-linha">
        <button onclick="limpar()">Limpar</button>
    </div>

    <div class="segunda-linha">
        <button onclick="calcularequacaodareta()">Equação da Reta</button>
    </div>


<script src="javascript/equacaoReduzida.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora</title>
    <link rel="stylesheet" href="css/menu.css">
    <link rel="stylesheet" href="css/calculadora.css">
</head>
<body onkeypress="clicouTecla(event)">
<nav>
    <a href="index.html" class="selecionada">Clássica</a>
    <a href="equaçaoEntreDoisPontos.html">Equação entre Dois Pontos</a>
    <a href="distanciaEntrePontoeReta.html">Distância entre Ponto e Reta</a>
    <a href="equaçaoReduzida.html">Equação Reduzida</a>
    <a href="posiçaoRelativadasRetas.html">Posição Relativa das Retas</a>
</nav>

<div class="calculadora">
    <input type="text" disabled class="display" id="display">
    <div class="primeiros-botoes">
            <button onclick="limpar()">LIMPAR</button>
            <button onclick="backspace()"><<</button>
            <button onclick="selecionarOperacao('/')">/</button>
    </div>
    <div class="botoes-centrais">
        <button onclick="inserirNumero('7')">7</button>
        <button onclick="inserirNumero('8')">8</button>
        <button onclick="inserirNumero('9')">9</button>
        <button onclick="selecionarOperacao('*')">*</button>
        <button onclick="inserirNumero('4')">4</button>
        <button onclick="inserirNumero('5')">5</button>
        <button onclick="inserirNumero('6')">6</button>
        <button onclick="selecionarOperacao('-')">-</button>
        <button onclick="inserirNumero('1')">1</button>
        <button onclick="inserirNumero('2')">2</button>
        <button onclick="inserirNumero('3')">3</button>
        <button onclick="selecionarOperacao('+')">+</button>
    </div>
    <div class="ultimos-botoes">
        <button onclick="inserirNumero('0')">0</button>
        <button onclick="inserirDecimal()">,</button>
        <button onclick="chamarIgual()">=</button>
    </div>
</div>

<script src="javascript/classica.js"></script>

</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora rafinha</title>
    <link rel="stylesheet" href="css/menu.css">
    <link rel="stylesheet" href="css/calculadora.css">
    <link rel="stylesheet" href="css/posicaorelativadareta.css">

</head>
<body>

<nav>
    <a href="index.html">Clássica</a>
    <a href="equaçaoEntreDoisPontos.html">Equação entre Dois Pontos</a>
    <a href="distanciaEntrePontoeReta.html">Distância entre Ponto e Reta</a>
    <a href="equaçaoReduzida.html">Equação Reduzida</a>
    <a href="posiçaoRelativadasRetas.html" class="selecionada">Posição Relativa das Retas</a>

</nav>
<div class="calculadora">
    <input type="text" disabled class="display" id="display">


    <div class="pontos">
        <label>1° Reta</label>
        <div><span>M:</span><input type="number" name="" class="ponto" id="M"></div>
        <div><span>N:</span><input type="number" name="" class="ponto" id="N"></div>
    </div>
    <div class="pontos">
        <label>2° Reta</label>
        <div><span>M:</span><input type="number" name="" class="ponto" id="M1"></div>
        <div><span>N:</span><input type="number" name="" class="ponto" id="N1"></div>
    </div>
    <div class="primeira-linha">
        <button onclick="limpar()">LIMPAR</button>
    </div>

    <div class="segunda-linha">
        <button onclick="PosicaoR()">Posição Relativa Das Retas</button>
    </div>

<script src="javascript/posicaorelativadareta.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora rafinha</title>
    <link rel="stylesheet" href="css/menu.css">
    <link rel="stylesheet" href="css/calculadora.css">
    <link rel="stylesheet" href="css/distanciaEntrePontoeReta.css">

</head>
<body>

<nav>
    <a href="index.html">Clássica</a>
    <a href="equaçaoEntreDoisPontos.html">Equação entre Dois Pontos</a>
    <a href="distanciaEntrePontoeReta.html" class="selecionada">Distância entre Ponto e Reta</a>
    <a href="equaçaoReduzida.html">Equação Reduzida</a>
    <a href="posiçaoRelativadasRetas.html">Posição Relativa das Retas</a>
</nav>

<div class="calculadora">
    <input type="text" disabled class="display" id="display">

    <div class="pontos">
        <label> Ponto A</label>
        <div><span>X:</span><input type="number" class="ponto" id="xPontoA"></div>
        <div><span>Y:</span><input type="number" class="ponto" id="yPontoA"></div>
    </div>

    <div class="equacao">
        <label> Ponto B</label>
        <div><span>A:</span><input type="number" class="ponto" id="PontoA"></div>
        <div><span>B:</span><input type="number" class="ponto" id="PontoB"></div>
        <div><span>C:</span><input type="number" class="ponto" id="PontoC"></div>
    </div>

    <div class="primeira-linha">
        <button onclick="limpar()">Limpar</button>
    </div>

    <div class="segunda-linha">
        <button onclick="calcularDistanciadePontoeReta ()">Distância Entre Ponto e Reta</button>
    </div>


<script src="javascript/distanciaEntrePontoeReta.js"></script>
</body>
</html>
