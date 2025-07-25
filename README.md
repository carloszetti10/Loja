# Loja

Crie um arquivo FXML chamado `Main.fxml` para uma aplicação JavaFX, que será usada como tela principal de um sistema de gerenciamento de curso.

Estrutura:
- Use `HBox` como layout raiz.
- Do lado esquerdo, crie uma barra lateral (`VBox`) com largura fixa para navegação.
- Do lado direito, use um `StackPane` com `HBox.hgrow="ALWAYS"` e `fx:id="contentView"` para exibir as telas dinamicamente.

A barra lateral (sidebar) deve conter os seguintes botões de menu, um embaixo do outro:
1. Tela Inicial  
2. Configuração  
3. Relatórios  
4. Gerenciamento de Chaves  
5. Sair

Cada botão do menu deve ser um `VBox` com:
- Um `SVGPath` (ícone)
- Um `Label` com o texto correspondente
- Atributo `onMouseClicked="#clickMenu"`
- Atributo `id` com o nome da seção (ex: "TelaInicial", "Configuracao", etc.)
- A classe CSS `side-bar-menu`

Estilo:
- O `HBox` raiz deve ter a classe `main-frame`
- O menu lateral (`VBox`) deve ter a classe `side-bar`
- Cada item deve usar `side-bar-menu`
- A folha de estilo externa deve ser `stylesheets="@style/application.css"`
- Use espaçamento interno (padding), espaçamento entre os itens (spacing), e visual limpo
- Não usar `layoutX` nem `layoutY`, apenas layout baseado em `VBox`, `HBox`, e propriedades responsivas

Extras:
- Defina o `fx:controller="com.seuprojeto.controller.MainController"`
- Adicione `xmlns:fx="http://javafx.com/fxml"` no nó raiz
- Use apenas componentes JavaFX nativos
- Gere **apenas o conteúdo do FXML**, sem código Java

Objetivo:
Essa tela servirá como container principal do sistema. O conteúdo do `StackPane` será trocado ao clicar nos menus.
- O `StackPane` deve ter `fx:id="contentView"` para carregar dinamicamente outras telas FXML.
- A barra lateral deve ter `fx:id="sideBar"` e cada item deve ter um `id` único e atributo `onMouseClicked="#clickMenu"`.
- Use `xmlns:fx="http://javafx.com/fxml"` e `fx:controller="com.projeto.domRio1.doRio.controller.MainController"`.
- Inclua um link para uma folha de estilo externa com `stylesheets="@style/application.css"` e defina a classe CSS raiz como `main-frame`.

Requisitos adicionais:
- Remova qualquer `layoutX` ou `layoutY` fixo para garantir responsividade.
- Use apenas elementos nativos do JavaFX.
- Gere apenas o conteúdo FXML, sem código Java.
