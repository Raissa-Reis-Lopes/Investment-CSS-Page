Porjeto realizado como conclusão das aulas de CSS na Alpha EdTech!




Orientações para a realização do projeto:

Projeto de aplicação com CSS

Chegamos ao final do módulo, e nada melhor do que um projeto para medirmos o nosso aprendizaddo!
Para tal, você deverá criar uma Landing Page!

Por definição, uma landing page consiste numa página destinada a instigar os usuários a comprar
determinado produto ou a contratar determinado serviço. Mais detalhes podem ser encontrados nessa
referência: https://resultadosdigitais.com.br/marketing/o-que-e-landing-page/.

Sua tarefa será escolher um produto ou serviço para promover e construir uma landing page para esse
produto ou serviço.

Considere e utilize todo o conhecimento que você obteve até o momento, sobre HTML e CSS.

Alguns critérios devem ser considerados:
  ● A página deve conter todos os atributos essenciais para uma página profissional, o que inclui não
  menos do que:
      ○ título e ícone (favicon)
      ○ metadados de descrição e palavras-chave
      ○ Open Graph
      ○ tags semâticas
  ● Estilize sua página com todo o conhecimento obtido no módulo de CSS, tomando como obrigatório
  a aplicação das seguintes tecnologias:
      ○ estruturação com Flexbox e/ou Grid Layuot
      ○ fontes externas, com Google Fonts ou similares
      ○ configuração do tema da página com uso de variáveis CSS
      ○ animações
      ○ responsividade


A página também deve possuir um design agradável e cores harmônicas. Para isso, utilize os conceitos
aprendidos sobre cores ou leve em consideração as cores de um design já existente.


A responsividade da página deve ser configurada considerado o conceito Mobile First. Caso seja
necessário adicionar ação a um botão de menu, você pode seguir o seguinte passo a passo:
    ● Adicione uma tag script ao HTML da sua página, como a seguir:
          <body>
           ...
           <script type="application/javascript" src="index.js" ></script>
          </body>
          index.html
  ● Crie um arquivo index.js e cole o seguinte script:

        const menu = document.querySelector ("#<id do menu>" )
        const openButton = document.querySelector ("#<id do botão que exibe o menu>" )
        const closeButton = document.querySelector ("#<id do botão que oculta o menu>" )
        document.querySelector ("#open").addEventListener ("click", function (){
         menu.style.display = "flex";
         openButton.style.display = "none";
         closeButton.style.display = "flex";
        })
        document.querySelector ("#close" ).addEventListener ("click", function (){
         menu.style.display = "none";
         openButton.style.display = "flex";
         closeButton.style.display = "none";
        })
  
   Para entendimento:
  ❖ A expressão document.querySelector(<seletor>), seleciona um elemento HTML, de
  acordo com o seletor especificado, assim como o seletores na folha de estilo
  ❖ A função addEventListenner(“action”, function() { … }), executa uma função sempre
  que uma ação é realizada em um elemento
  ❖ O atributo style.display armazena o valor da propriedade display do elemento HTML
  ● No script acima, substitua as expressões indicadas com os símbolos <> pelos seletores
  especificados. 
