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