<body>

<header>ALURAFLIX</header>


<h1>ATRAVÉS DO ARANHAVERSO SUPERA O PRIMEIRO FILME?</h1>
<p>#homem-aranha</p>



<iframe width="560" height="315" src="https://www.youtube.com/embed/gt_fAE1Eg2Q?si=c93nZtO1DTNYueO4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



<body> 
<body>
    <header>ALURAFLIX</header>

    <h1>ATRAVÉS DO ARANHAVERSO SUPERA O PRIMEIRO FILME?</h1>
    <p>#homem-aranha</p>

    <iframe width="560" height="315" src="https://www.youtube.com/embed/gt_fAE1Eg2Q?si=EEv-tsY_b1B2OwKE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

</body>
    <main>
        <div class="passo ativo" id="passo-0">
            <p>Um dia desses, dentro de um livro da biblioteca da escola, descobri uma carta antiga sobre uma cidade perdida, escondida por riquezas e belezas naturais. Nessa carta, a autora deixa algumas pistas para encontrar essa cidade e eu decidi segui-las!</p>
            <button class="btn-proximo" data-proximo="1">Rio de Janeiro</button>
            <button class="btn-proximo" data-proximo="2">Pernambuco</button>
        </div>
        <div class="passo" id="passo-1">
            <p>Você começa sua jornada no Rio de Janeiro, subindo o Pico da Tijuca ao amanhecer para encontrar a primeira pista.</p>
            <button class="btn-proximo" data-proximo="3">Procurar a pista no topo do pico</button>
            <button class="btn-proximo" data-proximo="4">Desistir e voltar para casa</button>
        </div>
        </main>

body {
    background-color: #1D4221;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 700px;
    margin: 0;
}

button {
    background-color: #64A712;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
}
const avanca = document.querySelectorAll('.btn-proximo');

avanca.forEach(button => {
    button.addEventListener('click', function(){
        const atual = document.querySelector('.ativo');
        const proximoPasso = 'passo-' + this.getAttribute('data-proximo');

        atual.classList.remove('ativo');
        document.getElementById(proximoPasso).classList.add('ativo');
    })
})

