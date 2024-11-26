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