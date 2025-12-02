## Exercícios de Criação de Páginas com HTML, CSS e JavaScript


### 1. Criador de Cartão de Perfil Interativo

Este exercício foca na estrutura básica, estilização e manipulação simples de conteúdo.

#### Passos:

1.  **Estrutura HTML (`index.html`):** Crie a estrutura básica para um cartão de perfil. O cartão deve incluir:
    * Um título/nome.
    * Uma imagem de perfil (use um *placeholder*).
    * Um parágrafo de biografia.
    * Um botão com o texto "Mostrar Detalhes".
2.  **Estilização CSS (`style.css`):**
    * Estilize o cartão para que tenha um fundo colorido ou sombra, centralizando-o na tela.
    * Defina um estilo para a imagem de perfil (ex: circular).
    * Defina um estilo inicial para a área de detalhes (ex: `display: none;`).
3.  **Funcionalidade JavaScript (`script.js`):**
    * Adicione um **ouvinte de evento** ao botão "Mostrar Detalhes".
    * Ao clicar, altere o estilo da área de detalhes para que ela seja **visível**.
    * **Desafio:** Mude o texto do botão para "Ocultar Detalhes" quando os detalhes estiverem visíveis e vice-versa.

---

### 2. Lista de Tarefas (To-Do List) Simples

Este exercício trabalha a manipulação do DOM e a interação com formulários.

#### Passos:

1.  **Estrutura HTML (`index.html`):** Crie uma seção de *To-Do List* contendo:
    * Um formulário com um campo de entrada (`<input type="text">`) e um botão "Adicionar".
    * Uma lista não ordenada (`<ul>` ou ordenada `<ol>`) vazia, onde as tarefas serão exibidas.
2.  **Estilização CSS (`style.css`):**
    * Estilize o formulário e o botão.
    * Estilize os itens da lista para que pareçam tarefas, talvez com um pequeno espaçamento ou borda.
    * **Opcional:** Adicione um estilo para marcar uma tarefa como concluída (ex: linha através do texto - *strikethrough*).
3.  **Funcionalidade JavaScript (`script.js`):**
    * Adicione um **ouvinte de evento** ao formulário para que, ao ser enviado:
        * O texto do campo de entrada seja capturado.
        * Um novo item da lista (`<li>`) contendo o texto da tarefa seja criado.
        * O novo item seja anexado à lista na tela.
        * O campo de entrada seja limpo.
    * Adicione um **ouvinte de evento** a cada novo item da lista para que, ao ser clicado, ele **alterne** a classe CSS de "concluído".

---

### 3. Galeria de Imagens com Zoom na Visualização

O foco aqui é na manipulação dinâmica de atributos e eventos de *mouseover*.

#### Passos:

1.  **Estrutura HTML (`index.html`):** Crie dois contêineres principais:
    * Um para a **imagem de visualização principal** (uma tag `<img>` maior).
    * Um para as **miniaturas** (várias tags `<img>` menores, cada uma com o atributo `data-full-src` apontando para a imagem grande). Use URLs de *placeholder* ou imagens próprias.
2.  **Estilização CSS (`style.css`):**
    * Estilize a imagem de visualização principal (tamanho fixo, borda).
    * Estilize as miniaturas para que sejam pequenas e tenham um efeito visual ao passar o mouse (ex: opacidade reduzida ou borda).
3.  **Funcionalidade JavaScript (`script.js`):**
    * Para **cada miniatura**: adicione um **ouvinte de evento** para o evento `click`.
    * Quando uma miniatura for clicada, o **atributo `src`** da imagem de visualização principal deve ser atualizado para o valor do atributo `data-full-src` da miniatura clicada.
    * **Desafio:** Adicione um **ouvinte de evento** de `mouseover` (`mouseenter`) às miniaturas para mostrar um *preview* no visualizador principal sem precisar clicar.

---

### 4. Contador Regressivo Simples

Este exercício utiliza funções de tempo (`setTimeout`/`setInterval`) e formatação de texto.

#### Passos:

1.  **Estrutura HTML (`index.html`):** Crie uma interface com:
    * Um elemento (`<span>` ou `<div>`) para exibir o **tempo restante** (ex: "00:10").
    * Um botão "Iniciar".
    * Um botão "Parar".
2.  **Estilização CSS (`style.css`):**
    * Estilize o número do contador para ser grande e centralizado, talvez com uma cor de destaque.
    * Estilize os botões.
3.  **Funcionalidade JavaScript (`script.js`):**
    * Crie uma variável para armazenar o tempo inicial (ex: 10 segundos).
    * Crie uma função que **decrementa** o tempo a cada segundo usando `setInterval()`.
    * A cada decremento, atualize o texto no HTML.
    * Adicione um **ouvinte de evento** ao botão "Iniciar" para começar o `setInterval()`.
    * Adicione um **ouvinte de evento** ao botão "Parar" para parar o `setInterval()` usando `clearInterval()`.
    * **Condição de parada:** O contador deve parar e exibir uma mensagem (ex: "Tempo Esgotado!") quando atingir 0.

---

### 5. Alternador de Tema (Light/Dark Mode)

Este exercício explora a manipulação de classes no elemento `<body>` para alternar estilos globais.

#### Passos:

1.  **Estrutura HTML (`index.html`):** Crie uma página de conteúdo simples (título, parágrafos) e um botão de alternância (ex: um ícone de sol/lua ou um *checkbox*).
2.  **Estilização CSS (`style.css`):**
    * Defina os estilos de tema **claro** (*default*): fundo claro, texto escuro.
    * Crie uma classe CSS chamada `.dark-mode` (ou similar) que **inverte** esses estilos (fundo escuro, texto claro).
    * Adicione estilos para que a transição de cores seja suave (ex: usando a propriedade `transition`).
3.  **Funcionalidade JavaScript (`script.js`):**
    * Adicione um **ouvinte de evento** ao botão/checkbox de alternância.
    * Ao clicar, use a propriedade `classList.toggle()` no elemento **`<body>`** para adicionar ou remover a classe `.dark-mode`.
    * **Persistência (Desafio):** Use o **`localStorage`** do navegador para salvar a preferência de tema do usuário e aplicá-la automaticamente quando a página for recarregada.
