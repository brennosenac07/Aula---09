# React Components 

*Brenno Elimar*

Inicialmente, baixe e extraia o arquivo images.zip fornecido. Em seguida, abra uma pasta assets na pasta pública do seu projeto React e transfira a pasta de imagens para o diretório public/assets. Essas imagens serão empregadas para mostrar os pratos no elemento de menu

Crie uma nova pasta chamada components na pasta src. Depois, adicione um arquivo a essa pasta, No MenuComponent.js. Este componente será encarregado de apresentar dinamicamente a lista de pratos, utilizando informações como nome, descrição e imagem de cada prato

Depois de desenvolver o componente de menu, acesse o arquivo App.js e insira o MenuComponent nele. Em seguida adicione o componente ao JSX, de modo que o menu seja apresentado na interface do aplicativo

Abra o arquivo App.css e apague qualquer conteúdo já presente, já que este exercício não requer estilos personalizados no momento

Após realizar todas as alterações no código, salve as mudanças e faça um commit no Git com a seguinte mensagem: "Components Part 1"

# Explicando o código

O código especifica um componente React conhecido como Menu, que apresenta uma lista de pratos por meio da biblioteca reactstrap. Ele usa o método useState para guardar as informações dos pratos em um array de objetos, cada um contendo dados como nome, imagem, categoria, preço e descrição.
O método map() mapeia a lista de pratos, resultando em um elemento JSX estruturado para cada prato, utilizando o componente Media do reactstrap. Cada item contém uma imagem (renderizada à esquerda com o objeto Media) e texto (nome e descrição) apresentados no corpo do documento (Media body).

# Aula - 10

# MenuComponent.js
**Quais os imports utilizados?**
React e useState (do React) - Para criar o componente e gerenciar estado.
Card, CardImg, CardImgOverlay, CardText, CardBody, CardTitle (do Reactstrap) - Para criar e estilizar os elementos visuais do menu.

**Há componentes? O que fazem?**
Sim, o código possui componentes. O principal é o `Menu`, que é responsável por exibir uma lista de pratos e os detalhes do prato selecionado. Além disso, ele utiliza componentes do Reactstrap como `Card`, que organiza as informações do prato, `CardImg`, que exibe a imagem, `CardImgOverlay`, para sobrepor textos na imagem, `CardBody`, que agrupa o conteúdo interno do card, `CardTitle`, para o título do prato, e `CardText`, que apresenta a descrição.

**Para que serve o onDishSelect no projeto?**
O `onDishSelect` é responsável por atualizar o estado `selectedDish` com o prato que o usuário clicou, permitindo exibir os detalhes desse prato.

**Para que serve o renderDish?**
O renderDish é responsável por exibir os detalhes do prato selecionado, como imagem, nome e descrição. Se nenhum prato for selecionado, ele retorna um elemento vazio.

**Para que serve o props.dishes.map?**
O `props.dishes.map` é usado para iterar sobre a lista de pratos recebida como propriedade (`dishes`) e gerar um card para cada prato, exibindo sua imagem e nome na interface.


# dishes.js
**Quais as propriedades?**
Cada prato possui propriedades como *id*, *name*, *image*, *category*, *label*, *price*, *description* e *comments*. A propriedade *comments* contém uma lista com *id*, *rating*, *comment*, *author* e *date* para cada comentário relacionado ao prato.

**que tipo de date é utilizado?**
O tipo de date utilizado é uma string no formato ISO 8601.


# Apps.js
**Para que serve oconst [dishes]?**
o [dishes] usa o Hook useState para armazenar o array de pratos (DISHES) no estado do componente App.

**Explicar como funciona o <Menu dishes={dishes} />**
O `<Menu dishes={dishes} />` passa o array `dishes` como uma prop para o componente `Menu`. No `Menu`, essa prop é usada para renderizar a lista de pratos dinamicamente.
