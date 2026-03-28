# nutritionist-website
My first frontend project built with HTML and CSS without AI assistance. A simple nutritionist website with profile information and appointment button.

<!DOCTYPE html>
<html lang="pt-br">
<head>
  <link rel="Stylesheet" type="text/css" href="estilo.css">
<meta charset="utf-8">
<title>Leandro Fernandes, o seu Nutri   </title>
</head>
<body>
  <div class="faixa">
  <div class="logo-area">
    <img src="logo.nutri-png.png" alt="Logo Leandro Fernandes">
    <span>Leandro Fernandes</span>
  </div>
  </div> 
  <div class="sobre">
    <figure class="foto-do-leandro">
      <img src="leandro.nutri.semFundo.png">
      <figcaption class="conhecaSeuNutri">
        <h1>Conheça o Seu Nutri</h1>
    </figcaption>
    </figure>
  <div class="conteudo">  
    <h2 class="agendeja">AGENDE JÁ UMA CONSULTA COM O SEU NUTRICIONISTA</h2>      
    <div class="formacao">
      <h2 class="conheca">Sobre mim:</h2>
      <h2>Formação</h2>
        <p>Formado em Nutrição pela Universidade Federal do Ceará</br> 
        e Pós-graduando em Nutrição Clínica, Esportiva e Fitoterapia.</p>
  </div>
  <div class="especialidade">   
    <h2>Área Especializada:</h2>
      <p>
      Foco em emagrecimento saudável, nutrição clínica e performance esportiva, 
      com atendimento personalizado para cada paciente. 
      O objetivo é promover resultados duradouros através de uma alimentação equilibrada, 
      melhorando a saúde, o bem-estar e o desempenho físico no dia a dia.</p>  
  </div>  
  </div>        
  </div>
  <div class="motivador">
    <H1>Minha missão é promover mudanças positivas na sua vida 
    através de nutrição e atividade física</H1>
      <h2>Tenha todo suporte e orientação para que você alcance
        seus objetivos de forma saudável e sustentável.</h2>
  </div>  
  <div class="agendar">
    <h1>AGENDE AGORA UMA CONSULTA COM SEU NUTRICIONISTA!</h1>
  <div class="seta"></div>
    <div class="botao-centro">
      <button class="btn">
      <img src="whatsapp-removebg.png" class="icon">
        Agendar Consulta
      </button>
    </div>
  </div>
  </div>
</body>
</html>

@charset "UTF-8";
body {
    background-color: white;
    padding-top: 180px;
  }
  h1 {
    font-size: 45px;
    text-align: center;
  }
  h2 {
    font-size: 40px;
    text-align: center;
    margin-top: 0px;
}
 p {
    text-align: justify;
    margin-bottom: 20px;
    font-size: 35px;
}
.faixa {
    /*altura fixa*/
    height: 100px;
    display: flex;
    /*centraliza verticalmente*/
    align-items: center;
    position: fixed;
    top: -15px;
    left: 0;
    width: 100%;
    background-color: #D2B48C;
    color: white;
    border-bottom: 2px solid rgba(0,0,0,0.1);
    padding: 10px 20px;
    text-align: center;
    letter-spacing: 5px;
    z-index: 1000;
}
.logo-area {
    display: flex;
    align-items: center;
    gap: 10px;
}
.logo-area img {
    margin-bottom: -60px;
    width: 360px;
}
.logo-area span {
    letter-spacing: normal;
    font-size: 50px;
    font-weight: bold;
    color: white;
}
.sobre {
    background-color: white;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 40px;
    gap: 20px;
    margin-top: 370px;
}
figure.foto-do-leandro {
    margin-left: -500px
    position: relative;
    margin-top: -900px;
    margin-left: -300px;

}
figure.foto-do-leandro img{
    background-color: white;
    max-width: 900px;
}
figure.foto-do-leandro figcaption {
    background-color: white;
}
.conhecaSeuNutri {
    background-color: white;
    margin-right: -70px;
}
.agendeja {
    white-space: nowrap; /*impede que o texto quebre em várias linhas, mantendo tudo em uma linha só*/
    font-size: clamp(20px, 5vw, 40px); /*tamanho do texto responsivo, adaptando-se ao tamanho da tela*/
    text-align: left;
    margin-left: -400px;
    margin-bottom: 100px;
}
.conteudo {
    background-color: white;
    max-width: 800px;
    margin-top: -450px;
}
.formacao{
    background-color: white;
}
.especialidade {
    background-color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 350px;
}
.motivador {
    background-color: white;
    margin-top: 300px;
}
.agendar {
    white-space: nowrap;
    text-align: justify;
    color: white;
    margin-top: 30px;
    background-color: #90EE90; 
    padding: 20px 0;
    border-radius: 45px;
}
.seta {
    width: 50px;
    height: 50px;
    border-right: 3px solid black;
    border-bottom: 3px solid black;
    transform: rotate(45deg);
    margin: 20px auto;
  }
.botao-centro {
    background-color: #90EE90;
    display: flex; /*faz com que tudo dentro do botão fique em linha lado a lado por padrão*/
    justify-content: center; /*alinha o botao no meio da tela*/
    margin-top: 20px; /*separar o botao do conteúdo acima, dando espaçamento*/
    margin-bottom: 20px;
}
.btn {
    display: flex;
    align-items: center;
    gap: 10px;
    background-color: #28a745; /*cor de fundo do botão*/
    color: white; /*cor do texto dentro do botão*/
    transition: 0.3s; /*faz qualquer mudança acontecer de forma suave, sem mudar do nada*/
    padding: 12px 25px; /*espaço interno dentro do botão*/
    border: none; /*remove a borda do botão*/
    cursor: pointer; /*muda o cursor do mouse para "maozinha" ao passar por cima do botão*/
    font-size: 30px; /*tamanho do texto*/
    border-radius: 45px; /*arredondar as bordas do botão*/
}
.btn:hover { /*funçao que se ativa apenas quando passa o mouse por cima*/
    background-color: #218838;
    color: white;
}
.icon {
    background-color: green;
    width: 70px;
}
transform: scale(1.05); /*efeito visual, aumenta o botão, parecendo que ele "cresce"*/
