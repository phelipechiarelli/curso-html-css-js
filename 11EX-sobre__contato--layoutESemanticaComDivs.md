# Exercício: Um pouco sobre estilização com blocos

## Objetivo
      
Primeiro vamos criar as classes que serão utilizadas no CSS para estilizar as informações de telefones. Precisamos deixar ambas as informações na mesma linha:
Ex: `Pessoa Física: (11) 4118-3319`

## Passo a passo com código

1. No arquivo **`sobre.css`** na pasta **`css`** faça as seguintes alterações:

    ###### # css/sobre.css
    ```css
     body {
       width: 940px;
       margin-left: auto;
       margin-right: auto;
     
       font-family: "Helvetica", "Lucida Grande", sans-serif;
       color: #3D3D3D;
     }
     
     .titulo {
       padding: 10px;
     
       font-size: 32px;
     
       background-color: #E1EDF2;
     }
     
     .subtitulo {
       border-bottom: 2px solid black;
     }
     
     figure {
       margin: 30px;
       padding: 15px;
       
       text-align: center;
     
       background-color: whitesmoke;
       border: 1px solid lightgrey;
     }
     
     figcaption {
       margin-top: 10px;
     }
     
     .matriz-musicdot {
       width: 550px;
       margin-left: auto;
       margin-right: auto;
     }
     
     .familia-tupfeln {
       width: 275px;
       float: right;
     }
     
     figure img {
       width: 100%;
     }
     
     .contato__subtitulo {
       display: inline;
     }
     
     .contato__info {
       margin: 16px 0 24px;
       padding-left: 32px;
     }
    +
    +.contato__info-titulo,
    +.contato__info-descricao {
    +  display: inline;
    +}
    +
    +.contato__info-descricao {
    +  margin-left: 10px;
    +}
    ```

2. No arquivo **`sobre.html`** na pasta **`raíz do projeto`** faça as seguintes alterações:

    ###### # sobre.html
    ```html
     <!doctype html>
     <html lang="pt-BR">
       <head>
         <meta charset="utf-8">
         <title>
           MusicDot | Sobre a empresa
         </title>
         <link href="img/favicon.ico" rel="icon">
         <link rel="stylesheet" href="css/sobre.css">
       </head>
       
       <body>
         
         <img src="img/logo.svg" alt="MusicDot">
     
         <h1 class="titulo"> Sobre a empresa </h1>
     
         <p>
           A MusicDot é a maior escola online de música em todo o mundo.
           Fundada em 1932, possui estúdios em 124 países, sendo líder de mercado com mais de 90% de
           participação em 118 deles.
         </p>
         
         <p>
           Nossa matriz fica em <a href="https://maps.google.com.br/?q=190,GabrielDequech,Mafra,SC"> Mafra, em Santa Catarina </a>. De lá, saem grande parte das gravações de nossos cursos. Nossa matriz:
         </p>
     
         <figure class="matriz-musicdot">
           <img src="img/matriz-musicdot.png" alt="Matriz da musicdot">
           <figcaption>
               Matriz MusicDot 
           </figcaption>
         </figure>
         
         <p>
           Assine os cursos da MusicDot. Acesse <a href="index.html"> nosso site </a> ou entre em contato
           se tiver dúvidas. Conheça também <a href="#historia"> nossa história </a> e <a href="#diferenciais"> nossos diferenciais </a>.
         </p>
     
         <h2 id="historia" class="subtitulo"> História </h2>
     
         <figure class="familia-tupfeln">
           <img src="img/familia-tupfeln.jpg" alt="Foto da família tüpfeln">
           <figcaption>Família Tüpfeln</figcaption>
         </figure>
         
         <p>
           A fundação em 1932 ocorreu no momento da descoberta econônica de cursos por stream online no interior de Santa Catarina. A
           família Tüpfeln, tradicional da região, investiu todas as suas economias nessa nova iniciativa,
           revolucionária para a época. A fundadora frau Dagmar Olaf Tüpfeln, dotada de particular visão
           administrativa, guiou os negócios da empresa durante mais de 50 anos, muitos deles ao lado
           de seu filho Ernst Noten Tüpfeln, atual CEO. O nome da empresa é inspirado no nome da família.
         </p>
         
         <p>
           O crescimento da empresa foi praticamente instantâneo. Nos primeiros 5 anos, já atendia 18 países.
           Bateu a marca de 100 países em apenas 15 anos de existência. Até hoje, já atendeu 2 bilhões
           de usuários diferentes, em bilhões de diferentes pedidos.
         </p>
         
         <p>
           O crescimento em número de funcionários é também assombroso. Hoje, é a maior empregadora do
           Brasil, mas mesmo após apenas 5 anos de sua existência, já possuía 30 mil funcionários. Fora do
           Brasil, há 240 mil funcionários, além dos 890 mil brasileiros nas instalações de Mafra e
           nos escritórios em todo país.
         </p>
         
         <p>
           Dada a importância econômica da empresa para o Brasil, a família Tüpfeln já recebeu diversos prêmios,
           homenagens e condecorações. Todos os presidentes do Brasil já visitaram as instalações da MusicDot, além de presidentes da União Européia, Ásia e o secretário-geral da ONU.
         </p>
     
         <h2 id="diferenciais" class="subtitulo"> Diferenciais </h2>
         <ul>
           <li> Menor preço do mercado, garantido </li>
           <li> Se você achar um serviço mais barato, leva 1 mês de graça </li>
           <li> Pague em reais, dólares, euros, libras, dodgecoins, litecoins ou bitcoins </li>
           <li> Todas as compras acompanham acesso à Alura </li>
           <li> Maior escola de música online do mundo </li>
           <li> Atendimento via telefone, email, chat, twitter, facebook, instagram, ICQ, WhatsApp, SMS, carta, fax, sinal de fumaça e telegrama </li>
           <li> Presente em 124 países </li>
           <li> Mais de um milhão de funcionários em todo o mundo </li>
         </ul>
         
         <h2 class="titulo"> Contato </h2>
     
         <h3 class="contato__subtitulo"> Correspondência </h3>
         <small> (todos os dias, das 9h às 18h) </small>
     
         <address class="contato__info">
             AOVS Sistemas de Informática S.A
             <br>
             Rua Vergueiro, 3185, 8º andar
             <br>
             Vila Mariana
             <br>
             São Paulo - SP
         </address>
     
         <h3 class="contato__subtitulo"> Telefones </h3>
         <small> (segunda à sexta, das 9h às 18h) </small>
         
         <dl class="contato__info">
    -      <̶d̶t̶>̶ P̶e̶s̶s̶o̶a̶ F̶í̶s̶i̶c̶a̶:̶ <̶/̶d̶t̶>̶
    -      <̶d̶d̶>̶ <̶a̶ h̶r̶e̶f̶=̶"̶t̶e̶l̶:̶/̶/̶1̶1̶4̶1̶1̶8̶-̶3̶3̶1̶9̶"̶>̶ (̶1̶1̶)̶ 4̶1̶1̶8̶-̶3̶3̶1̶9̶ <̶/̶a̶>̶ <̶/̶d̶d̶>̶
    -    
    -      <̶d̶t̶>̶ P̶e̶s̶s̶o̶a̶ J̶u̶r̶í̶d̶i̶c̶a̶:̶ <̶/̶d̶t̶>̶
    -      <̶d̶d̶>̶ <̶a̶ h̶r̶e̶f̶=̶"̶t̶e̶l̶:̶/̶/̶1̶1̶4̶1̶1̶8̶-̶2̶1̶7̶2̶"̶>̶ (̶1̶1̶)̶ 4̶1̶1̶8̶-̶2̶1̶7̶2̶ <̶/̶a̶>̶ <̶/̶d̶d̶>̶
    +      <div>
    +        <dt class="contato__info-titulo"> Pessoa Física: </dt>
    +        <dd class="contato__info-descricao"> <a href="tel://114118-3319"> (11) 4118-3319 </a> </dd>
    +      </div>
    +    
    +      <div>
    +        <dt class="contato__info-titulo"> Pessoa Jurídica: </dt>
    +        <dd class="contato__info-descricao"> <a href="tel://114118-2172"> (11) 4118-2172 </a> </dd>
    +      </div>
         </dl>
     
       </body>
     </html>
    ```
