## 20 Exercícios de Criação de Páginas com HTML, CSS e JavaScript

#### 1. Criador de Cartão de Perfil Interativo

Este exercício foca na estrutura básica, estilização e manipulação simples de conteúdo.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie a estrutura básica para um cartão de perfil, incluindo título, imagem de perfil, biografia e um botão "Mostrar Detalhes".
2.  **Estilização CSS (`style.css`):** Estilize o cartão (fundo, sombra, centralização). Defina um estilo para a imagem de perfil (ex: circular). Defina um estilo inicial para a área de detalhes (ex: `display: none;`).
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao botão "Mostrar Detalhes". Ao clicar, altere o estilo da área de detalhes para que ela seja **visível**. **Desafio:** Mude o texto do botão para "Ocultar Detalhes" e vice-versa.

#### 2. Lista de Tarefas (To-Do List) Simples

Este exercício trabalha a manipulação do DOM e a interação com formulários.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie uma seção de *To-Do List* contendo um formulário com campo de entrada e um botão "Adicionar", e uma lista não ordenada (`<ul>`) vazia.
2.  **Estilização CSS (`style.css`):** Estilize o formulário e os itens da lista. **Opcional:** Adicione um estilo para marcar uma tarefa como concluída (ex: linha através do texto).
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao formulário para que, ao ser enviado, crie e anexe um novo item da lista (`<li>`) com o texto da tarefa. Adicione um **ouvinte de evento** a cada novo item da lista para que, ao ser clicado, ele **alterne** a classe CSS de "concluído".

#### 3. Galeria de Imagens com Zoom na Visualização

O foco aqui é na manipulação dinâmica de atributos e eventos de *mouseover*.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um elemento para a **imagem de visualização principal** e um contêiner para as **miniaturas** (`<img>` menores). As miniaturas devem ter um atributo (ex: `data-full-src`) apontando para a imagem grande.
2.  **Estilização CSS (`style.css`):** Estilize a imagem principal e as miniaturas, incluindo um efeito visual nas miniaturas ao passar o mouse.
3.  **Funcionalidade JavaScript (`script.js`):** Para **cada miniatura**, adicione um **ouvinte de evento** para o evento `click`. Quando uma miniatura for clicada, o **atributo `src`** da imagem de visualização principal deve ser atualizado para o valor do atributo `data-full-src` da miniatura. **Desafio:** Adicione um **ouvinte de evento** de `mouseover` para mostrar um *preview* sem precisar clicar.

#### 4. Contador Regressivo Simples

Este exercício utiliza funções de tempo (`setTimeout`/`setInterval`) e formatação de texto.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie uma interface com um elemento para exibir o **tempo restante** (ex: "00:10") e botões "Iniciar" e "Parar".
2.  **Estilização CSS (`style.css`):** Estilize o número do contador para ser grande e centralizado, e estilize os botões.
3.  **Funcionalidade JavaScript (`script.js`):** Crie uma variável para o tempo inicial (ex: 10 segundos). Crie uma função que usa `setInterval()` para decrementar o tempo a cada segundo e atualizar o texto no HTML. Adicione **ouvintes de evento** para o botão "Iniciar" (começa o `setInterval`) e "Parar" (para o `setInterval` usando `clearInterval()`).

#### 5. Alternador de Tema (Light/Dark Mode)

Este exercício explora a manipulação de classes no elemento `<body>` para alternar estilos globais.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie uma página de conteúdo simples e um botão/checkbox de alternância.
2.  **Estilização CSS (`style.css`):** Defina os estilos de tema **claro** (*default*). Crie uma classe CSS chamada `.dark-mode` que **inverte** esses estilos (fundo escuro, texto claro).
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao botão de alternância. Ao clicar, use a propriedade **`classList.toggle()`** no elemento **`<body>`** para adicionar ou remover a classe `.dark-mode`. **Desafio:** Use o **`localStorage`** para salvar a preferência de tema do usuário.

#### 6. Validador de Formulário de Cadastro Simples

Este exercício foca na manipulação de eventos de formulário e validação de entrada de dados.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um formulário com campos de Nome de Usuário, Email, Senha, um botão de *submit* e um espaço para mensagens de erro.
2.  **Estilização CSS (`style.css`):** Estilize o formulário. Crie uma classe CSS (ex: `.erro`) para destacar a borda de um campo em vermelho quando a validação falhar.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao formulário para o evento **`submit`**, impedindo o comportamento padrão. Crie funções que validem as regras de cada campo (ex: mínimo de caracteres, presença de '@'). Se falhar, exiba a mensagem e adicione a classe `.erro`.

#### 7. Cronômetro Digital (Stopwatch)

Este exercício trabalha com manipulação de tempo e formatação numérica.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um elemento para exibir o tempo formatado (ex: "00:00:00") e três botões: "Iniciar", "Parar" e "Zerar".
2.  **Estilização CSS (`style.css`):** Estilize o mostrador do tempo para ser proeminente e os botões.
3.  **Funcionalidade JavaScript (`script.js`):** Crie variáveis para o tempo total decorrido e o ID do seu `setInterval`. Crie uma função que usa `setInterval()` para atualizar o tempo continuamente. Crie uma função de **formatação** que converte o tempo total em milissegundos para "HH:MM:SS". Adicione **ouvintes de evento** para "Iniciar" (começa), "Parar" (pausa com `clearInterval()`) e "Zerar".

#### 8. Alternador de Abas de Conteúdo (Tabbed Interface)

Este exercício foca em esconder/mostrar elementos usando classes CSS e lógica de cliques.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um contêiner de **botões/abas** e um contêiner para o **conteúdo**, com várias seções. Crie um **vínculo** entre os botões e as seções (ex: usando o atributo `data-target` no botão que corresponde ao `id` da seção).
2.  **Estilização CSS (`style.css`):** Estilize os botões. Crie uma classe `.active` para a aba selecionada. Defina o estilo padrão para que **todo o conteúdo das abas seja inicialmente oculto** (`display: none;`). Crie uma classe `.show` para torná-lo visível.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** para **todos** os botões de aba. Ao clicar, o JS deve: **Ocultar** todo o conteúdo, **Desativar** o destaque de todas as abas, **Ativar** o botão clicado e **Tornar visível** a seção de conteúdo correspondente.

#### 9. Notificação Flutuante Simples (Toast Message)

Este exercício envolve a criação dinâmica de elementos e a remoção programada.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um botão "Mostrar Notificação" e um contêiner vazio (`<div>`) fixo no canto inferior para as notificações.
2.  **Estilização CSS (`style.css`):** Estilize o contêiner de notificação para ser fixo. Crie classes para o visual da notificação. Crie classes CSS para adicionar e remover a notificação com animações.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao botão. Ao clicar, crie um **novo elemento `<div>`** dinamicamente para a notificação, defina seu conteúdo e anexe-o ao contêiner. Use **`setTimeout()`** para que, após 3 segundos, a notificação seja **removida do DOM**.

#### 10. Detector de Posição do Mouse

Este exercício foca em eventos de movimento e atualização de texto em tempo real.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie dois elementos separados (`<span>` ou `<p>`) para exibir a **Coordenada X** e a **Coordenada Y**.
2.  **Estilização CSS (`style.css`):** Estilize a página e destaque os elementos que exibem as coordenadas.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao objeto **`document`** ou **`<body>`** para o evento **`mousemove`**. Dentro da função de evento, acesse as propriedades **`event.clientX`** e **`event.clientY`** e use-as para **atualizar o `textContent`** dos elementos HTML correspondentes em tempo real.

#### 11. Filtro de Tabela Dinâmico

Este exercício explora a filtragem de dados em uma tabela HTML usando JavaScript.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie uma tabela HTML com dados fictícios e um campo de entrada de texto (`<input type="text">`) acima para filtrar.
2.  **Estilização CSS (`style.css`):** Estilize a tabela.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione um **ouvinte de evento** ao campo de entrada para o evento **`keyup`**. Crie uma função de filtro que itere sobre todas as linhas (`<tr>`) da tabela, verifique se o texto digitado está presente na coluna desejada (ignorando maiúsculas/minúsculas) e, se não estiver, defina o estilo da linha como **`display: none;`**.

#### 12. Seletor de Avaliação por Estrelas (Star Rating)

Este exercício foca na manipulação visual e na captura de valores usando eventos de mouse.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um contêiner vazio para as estrelas e um elemento de texto para exibir a pontuação atual.
2.  **Estilização CSS (`style.css`):** Use um **caractere Unicode de estrela** e crie duas classes CSS: uma para a **estrela vazia** e outra para a **estrela preenchida**.
3.  **Funcionalidade JavaScript (`script.js`):** Gere 5 elementos para as estrelas. Adicione um **ouvinte de evento** **`mouseover`** para **preencher** (adicionar a classe de cor) todas as estrelas até a posição atual do mouse. Adicione um **ouvinte de evento** **`click`** em cada estrela para **definir** a pontuação final e atualizar o texto na tela.

#### 13. Visualizador de Imagem com Controles de Zoom

Este exercício trabalha com a alteração do estilo para simular a funcionalidade de zoom.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie um contêiner com uma imagem (`<img>`) dentro e botões "Zoom +", "Zoom -" e "Resetar".
2.  **Estilização CSS (`style.css`):** Estilize a imagem. Defina a propriedade **`transition`** na imagem para que o zoom seja suave.
3.  **Funcionalidade JavaScript (`script.js`):** Crie uma variável global para rastrear o **nível de zoom atual** (ex: 1.0). Adicione **ouvintes de evento** aos botões para modificar o nível de zoom. Aplique o zoom à imagem usando a propriedade CSS **`transform: scale(X);`** (onde X é o nível de zoom).

#### 14. Lista com Arrastar e Soltar (Drag and Drop List)

Este exercício introduz os eventos nativos de *drag and drop* do HTML5.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie uma lista não ordenada de itens. Adicione o atributo **`draggable="true"`** a cada item da lista.
2.  **Estilização CSS (`style.css`):** Crie classes para fornecer *feedback* visual ao item que está sendo arrastado (`.dragging`) e para destacar a área onde um item pode ser solto (`.drag-over`).
3.  **Funcionalidade JavaScript (`script.js`):** Use os eventos **`dragstart`** (armazena referência), **`dragover`** (impede o comportamento padrão), **`drop`** (reordena os elementos no DOM) e **`dragend`** (remove o *feedback* visual).

#### 15. Gerador de Citação Aleatória

Este exercício combina a manipulação de *arrays* com a geração de números aleatórios.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Crie elementos para exibir o **texto da citação** e o **autor da citação**, além de um botão "Nova Citação".
2.  **Estilização CSS (`style.css`):** Estilize a citação e o autor.
3.  **Funcionalidade JavaScript (`script.js`):** Crie um **`Array` de Objetos** com citações e autores. Crie uma função que **gere um número inteiro aleatório** para selecionar um objeto de citação do *array*. Adicione um **ouvinte de evento** ao botão para chamar a função e atualizar o `textContent` dos elementos HTML.

#### 16. Carrossel de Imagens Simples

Este exercício foca na manipulação do **DOM** e na lógica de índice para navegação.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um contêiner com uma imagem `<img>` principal e botões "Anterior" e "Próximo".
2.  **Estilização CSS (`style.css`):** Defina o tamanho do carrossel. **Opcional:** Use `transition` para a troca suave de imagens.
3.  **Funcionalidade JavaScript (`script.js`):** Crie um **`Array`** de URLs de imagens e uma variável para rastrear o **índice** da imagem visível. Adicione **ouvintes de evento** aos botões para incrementar/decrementar o índice, garantindo que ele faça um **loop** (se passar do final, volta ao início, e vice-versa). Atualize o atributo **`src`** da imagem.

#### 17. Gerenciador de Notas Local (Usando `localStorage`)

Este exercício aprofunda o uso do **`localStorage`** para persistência de dados.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um campo de texto grande (`<textarea>`), um botão "Salvar Nota" e uma lista não ordenada (`<ul>`) para exibir as notas salvas.
2.  **Estilização CSS (`style.css`):** Estilize a área de texto, o botão e os itens da lista.
3.  **Funcionalidade JavaScript (`script.js`):** **Ao carregar a página:** Carregue e renderize as notas salvas no **`localStorage`**. Adicione um **ouvinte de evento** ao botão "Salvar Nota" para salvar a nota no `localStorage` e **renderizá-la** na lista na tela. **Desafio:** Implemente a funcionalidade de "Excluir" (remove do `localStorage` e do DOM).

#### 18. Simulador de Rolagem Infinita (Infinite Scroll)

Este exercício simula o carregamento de mais conteúdo à medida que o usuário se aproxima do final da página.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um contêiner de "Conteúdo" com alguns itens iniciais e um elemento de *loading* oculto no final.
2.  **Estilização CSS (`style.css`):** Estilize os itens de conteúdo e o indicador de *loading*.
3.  **Funcionalidade JavaScript (`script.js`):** Crie uma função `carregarMaisItens()` que cria e adiciona novos elementos de conteúdo. Adicione um **ouvinte de evento** ao objeto **`window`** para o evento **`scroll`**. Dentro do evento, compare o *scroll* do usuário com a altura total da página para detectar quando ele está perto do final e chame a função `carregarMaisItens()`.

#### 19. Gerador de Cores Aleatórias (Hex Color Generator)

Este exercício foca na geração de dados e na aplicação de estilos dinamicamente.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um contêiner principal, um elemento de texto **centralizado** para exibir o código hexadecimal da cor atual e um botão "Gerar Nova Cor".
2.  **Estilização CSS (`style.css`):** Estilize o contêiner para preencher a tela e o texto do código da cor.
3.  **Funcionalidade JavaScript (`script.js`):** Crie uma função para **gerar um código hexadecimal aleatório**. Adicione um **ouvinte de evento** ao botão para chamar a função e, em seguida, defina a propriedade **`backgroundColor`** do contêiner principal com o novo código de cor. Atualize o `textContent` do elemento centralizado.

#### 20. Alerta/Modal Personalizado

Este exercício aborda a criação de um modal (*pop-up*) que bloqueia a interação com o restante da página.

**Passos:**

1.  **Estrutura HTML (`index.html`):** Um botão "Mostrar Modal". Um contêiner grande (`<div>`) para o **fundo do modal** (overlay) e, dentro dele, a **caixa de conteúdo do modal** (com título, mensagem e botão "Fechar").
2.  **Estilização CSS (`style.css`):** Estilize o *overlay* para cobrir toda a tela com um fundo semi-transparente e **`position: fixed;`** (inicialmente `display: none;`). Estilize a caixa de conteúdo do modal para ser branca e **centralizada**. Crie uma classe `.show-modal` para tornar o *overlay* visível.
3.  **Funcionalidade JavaScript (`script.js`):** Adicione **ouvintes de evento** ao botão "Mostrar Modal" para adicionar a classe `.show-modal` e ao botão "Fechar" para removê-la. **Desafio:** Adicione um **ouvinte de evento** ao próprio *overlay* para que, ao clicar fora da caixa de conteúdo do modal, ele também se feche.


#### 21. Conversor de Moedas com Taxas Fixas
Este exercício foca em capturar valores numéricos de formulários, realizar operações matemáticas básicas e formatar a saída de dados.

**Passos**:

1. Estrutura HTML (index.html): Crie um campo de entrada numérico (<input type="number">) para o valor em Reais (BRL). Adicione um elemento de seleção (<select>) com opções de moedas de destino (ex: Dólar, Euro). Adicione um botão "Converter" e um elemento de texto para o resultado.

2. **Estilização CSS (style.css)**: Estilize o formulário de conversão de maneira limpa, destacando o campo de resultado.

3. **Funcionalidade JavaScript (script.js)**: Defina taxas de conversão fixas em variáveis ou em um objeto. Adicione um ouvinte de evento ao botão. Ao clicar, multiplique ou divida o valor inserido pela taxa da moeda selecionada e exiba o resultado formatado na tela.

#### 22. Jogo da Velha (Tic-Tac-Toe)
Este exercício trabalha fortemente com matrizes ou arrays de estado, detecção de padrões e alternância de turnos.

Passos:

**Estrutura HTML (index.html)**: Crie um contêiner principal para o tabuleiro e, dentro dele, 9 elementos individuais (ex: <div>) representando as casas do jogo. Adicione uma área de texto para indicar o jogador da vez ("Vez do X" ou "Vez do O") e um botão de reiniciar.

**Estilização CSS (style.css)**: Use CSS Grid no contêiner para criar uma grade de 3x3. Estilize as casas com bordas nítidas, tamanho fixo e cursor de clique.

**Funcionalidade JavaScript (script.js)**: Crie um array de 9 posições para rastrear o estado do tabuleiro e uma variável para o jogador atual ("X"). Adicione ouvintes de clique nas casas. Ao clicar em uma casa vazia, preencha-a com o símbolo atual, atualize o array de estado e verifique se há uma combinação vencedora (linhas, colunas ou diagonais). Se houver, declare o vencedor; caso contrário, alterne o turno.

#### 23. Barra de Progresso de Leitura
Este exercício utiliza o cálculo de posicionamento de rolagem da janela para atualizar uma propriedade visual em tempo real.

Passos:

**Estrutura HTML (index.html)**: Crie uma página com um texto longo (vários parágrafos para permitir rolagem). No topo da página, crie um contêiner para a barra de progresso com uma <div> interna vazia.

**Estilização CSS (style.css)**: Fixe o contêiner no topo da tela (position: fixed; top: 0; left: 0; width: 100%;). Dê à barra interna uma cor de destaque, altura pequena (ex: 5px) e largura inicial de 0%.

**Funcionalidade JavaScript (script.js)**: Adicione um ouvinte de evento ao objeto window para o evento scroll. Calcule a porcentagem da página que já foi rolada dividindo a posição atual do scroll (window.scrollY) pela altura total rolável do documento minus a altura da janela. Use essa porcentagem para atualizar dinamicamente a propriedade width da barra interna.

#### 24. Acordeão de Perguntas Frequentes (FAQ Accordion)
Este exercício foca na manipulação de elementos irmãos (sibling elements) e animações de expansão de altura.

Passos:

**Estrutura HTML (index.html)**: Crie uma lista de perguntas e respostas. Cada item deve ter um cabeçalho (a pergunta) e um painel de conteúdo (a resposta).

**Estilização CSS (style.css)**: Defina o painel de resposta com display: none; por padrão ou use propriedades de altura (height: 0; overflow: hidden;) combinado com transition para permitir efeitos suaves.

**Funcionalidade JavaScript (script.js)**: Adicione um ouvinte de evento de clique em todos os cabeçalhos de pergunta. Ao clicar em uma pergunta, verifique se o painel de resposta correspondente está aberto. Se estiver fechado, abra-o (e feche todos os outros painéis de resposta ativos na página).

#### 25. Calculadora de IMC com Feedback Visual
Este exercício exercita condicionais baseadas em faixas numéricas e manipulação de classes CSS para fornecer respostas visuais personalizadas.

Passos:

**Estrutura HTML (index.html)**: Crie dois campos de entrada numérica: um para o peso (kg) e outro para a altura (metros). Adicione um botão "Calcular" e uma área de texto para o resultado e a classificação.

**Estilização CSS (style.css)**: Crie classes de cores diferentes para os resultados (ex: verde para peso normal, amarelo para sobrepeso, vermelho para obesidade).

**Funcionalidade JavaScript (script.js)**: Adicione um ouvinte ao botão para efetuar o cálculo matemático do IMC (peso dividido pelo quadrado da altura). Utilize uma estrutura de if / else if para classificar o resultado obtido de acordo com as faixas padrão da OMS e mude a classe do elemento de resultado para a cor correspondente à classificação da pessoa.

#### 26. Filtro de Busca em Lista Textual (Live Search)
Este exercício aprimora a busca dinâmica comparando strings em tempo real à medida que o usuário digita.

Passos:

**Estrutura HTML (index.html)**: Crie um campo de entrada de texto para a pesquisa e uma lista simples (<ul> com vários <li>) contendo nomes de itens variados (ex: frutas, países ou filmes).

**Estilização CSS (style.css)**: Estilize a lista para uma leitura confortável e aplique efeitos visuais simples ao passar o mouse.

**Funcionalidade JavaScript (script.js)**: Adicione o evento input ou keyup no campo de busca. Na função associada, pegue o termo digitado, transforme-o em letras minúsculas e itere pelos itens da lista. Utilize funções de string (como includes()) para testar se o texto do item contém o termo digitado. Se não contiver, esconda o item aplicando uma classe ou alterando seu estilo diretamente.

#### 27. Botão de Curtir com Contador de Estados
Este exercício simula o comportamento comum de curtidas em redes sociais, trabalhando com variáveis booleanas e incrementos simples.

Passos:

**Estrutura HTML (index.html)**: Crie um contêiner representando uma postagem genérica. Dentro dele, adicione um botão de curtir (que pode conter texto ou um caractere representando um coração) e um elemento de texto indicando o número de curtidas (ex: "0 curtidas").

**Estilização CSS (style.css)**: Crie um estilo específico para quando o botão estiver no estado "curtido" (ex: mudando o fundo para azul ou vermelho).

**Funcionalidade JavaScript (script.js)**: Crie uma variável para contar o número de curtidas e uma variável booleana para registrar se o usuário atual já curtiu ou não o post. No clique do botão, faça a verificação: se o usuário ainda não curtiu, incremente o contador, marque a booleana como verdadeira e adicione a classe visual de curtido ao botão. Se ele clicar novamente, execute a ação inversa (decremento e remoção da classe).

#### 28. Medidor de Força de Senha em Tempo Real
Este exercício utiliza expressões regulares simples (RegEx) para analisar strings e atualizar componentes visuais dinamicamente.

Passos:

**Estrutura HTML (index.html)**: Crie um formulário com um campo de senha (<input type="password">). Abaixo do campo, crie uma <div> vazia que servirá de barra indicadora de força e um texto auxiliar.

**Estilização CSS (style.css)**: Crie uma barra base com largura total e fundo cinza. A barra interna de força deve ter transição suave de largura e cor.

**Funcionalidade JavaScript (script.js)**: Monitore o campo de senha com o evento input. Crie uma pontuação inicial de força igual a zero. Estabeleça testes na string da senha usando regras ou expressões regulares (ex: se contém mais de 8 caracteres, adicione +1 ponto; se contém números, +1 ponto; se contém caracteres especiais, +1 ponto; se contém letras maiúsculas, +1 ponto). Use a pontuação final para definir a largura (ex: 25%, 50%, 75%, 100%) e a cor da barra (vermelho, laranja, amarelo, verde).

#### 29. Sorteador de Números com Limites Customizados
Este exercício foca na manipulação do objeto matemático nativo do JavaScript e na validação lógica de intervalos numéricos.

Passos:

**Estrutura HTML (index.html)**: Crie dois campos de entrada numérica: "Mínimo" e "Máximo". Adicione um botão "Sortear" e um elemento com texto grande para exibir o número sorteado.

**Estilização CSS (style.css)**: Centralize os elementos na página e use fontes grandes e chamativas para exibir o número resultante do sorteio.

**Funcionalidade JavaScript (script.js)**: Adicione um ouvinte de evento ao botão. Capture os valores de mínimo e máximo, convertendo-os para números inteiros. Faça uma verificação para garantir que o valor máximo seja estritamente maior que o mínimo. Use funções matemáticas (como Math.random() e Math.floor()) para gerar um número inteiro aleatório que caia exatamente dentro do intervalo especificado pelo usuário e exiba-o no elemento de tela.

#### 30. Contador de Caracteres com Limite de Texto
Este exercício trabalha com a propriedade de comprimento de strings e o bloqueio visual ou textual de envio quando limites são excedidos.

Passos:

**Estrutura HTML (index.html)**: Crie uma área de texto (<textarea>) para digitação livre. Abaixo dela, coloque um pequeno elemento de texto para mostrar o balanço de caracteres (ex: "0 / 280 caracteres") e um botão "Publicar".

**Estilização CSS (style.css)**: Estilize o contador de caracteres de forma discreta. Crie uma classe CSS especial (ex: cor vermelha) para ser aplicada quando o usuário estiver muito próximo do limite ou se ultrapassá-lo.

**Funcionalidade JavaScript (script.js)**: Armazene o valor do limite máximo (ex: 280) em uma constante. Monitore as alterações da área de texto usando o evento input. A cada alteração, leia a propriedade .length do texto da área e atualize o elemento indicador na tela. Caso a contagem de caracteres ultrapasse o limite máximo estabelecido, adicione a classe visual vermelha ao texto do contador e desative o botão de publicação alterando sua propriedade .disabled.
