<!DOCTYPE html>
<!-- 
-->
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Namora comigo?</title>
</head>

<body>
    <div id="conteudo">
        <h2>desde que te conheci</h2>
	<h2>o dia de sol tem o céu mais azul </h2>
        <h2>nem to falando da lente de um óculos que parece intensificar as cores ♥.</h2>
	<h2> Eu amo muito você! mas...</h2>
	<h2>Voce aceitaria ser minha namorada?</h2>
	<button class="btn" onclick="sim()">SIM</button>
        <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)">NÃO</button>
    </div>
</body>
<style>
    #conteudo {
        background: #ff7a7a;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        text-align: center;
        font-family: sans-serif;
    }

    .btn {
        background: black;
        color: white;
        border: none;
        padding: 10px;
        width: 80px;
        border-radius: 5px;
    }
</style>

<script>
    function sim() {
        alert("Já sabia o que voce escolheria... te amo <3)");
        // redireciona para um URL após clicar no SIM
        location.href = "https://music.youtube.com/watch?v=izGwDsrQ1eQ";
    }

    function desvia(btn) {
        // btn declarado na função
        btn.style.position = 'absolute';
        btn.style.bottom = geraPosicao(10, 90);
        btn.style.left = geraPosicao(10, 90);
        console.log('opa, desviei...');
    }

    function geraPosicao(min, max) {
        return (Math.random() * (max - min) + min) + "%";
    }

    /* Apague se quiser, isso apenas escreve MTHS1901 e o link para o tutorial no console */
    const o = "MTHS1901", e = 90, l = "bold"; console.log(`%c${o}`, "font-size: 90px; font-weight: bold; background: linear-gradient(90deg, red, yellow);"), console.log("Tutorial: https://www.youtube.com/watch?v=zxxB9SFh9p4");

</script>

</html>
