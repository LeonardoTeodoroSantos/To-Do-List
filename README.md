# To-Do List

Um To-Do List nada mais é do que uma lista de afazeres, este app permite que você faça uma lista de tarefas, de coisas que você quer/precisa fazer.

## Descrição
Um app que permite que as pessoas que precisarem possam fazer uma lista de tarefas, para se organizarem e acompanharem com isso, o seu progresso nas tarefas.

## Tecnicas e Tecnologias Utilizadas
![Static Badge](https://img.shields.io/badge/HTML5-black?style=for-the-badge&logo=html5&logoColor=white&labelColor=%23E34F26&color=%23E34F26) ![Static Badge](https://img.shields.io/badge/CSS-black?style=for-the-badge&logo=css&logoColor=white&labelColor=%23663399&color=%23663399) ![Static Badge](https://img.shields.io/badge/JavaScript-black?style=for-the-badge&logo=javascript&logoColor=black&labelColor=%23F7DF1E&color=%23F7DF1E)

- `html`: HTML simples, somente o necessário para facilitar na estilização com o CSS e nas funções do JavaScript.


- `CSS`: CSS também simples, com alguns aprendizados novos, como a utilização do `background-image` buscando diretamente uma imagem na pasta da origem do projeto, sem usar a imagem através do HTML que foi só o que eu tinha visto até então. Também usando essa propriedade `background-image` para emular um checkbox, marcado e desmarcado. 


- `JavaScript`: JavaScript neste projeto ficou responsável por 4 funções, `Adicionar Tarefa`, `Marcar Tarefa como Concluída ou Excluir`, `Salvar Dados no localStorage` e `Carregar Dados Salvos`.  
  ### 1. Adicionar Tarefa
    <p align="center">
      <img src="https://github.com/user-attachments/assets/16861936-c66b-41f1-88df-18d8f7d7bf1b" width="50%">
    </p>
- Quando a função `addTask` é chamada através do botão `add` a função verifica se o input foi preenchido, se não, te pede para preencher. Preenchido o input a função cria um item de lista `li` e o adiciona ao container de tarefas `listContainer`.   
- Também é criado um elemento `span`, com o símbolo "X" funcionando como um botão para excluir uma tarefa caso necessário.
- Após adicionar a tarefa, o input é limpo e a função `saveData()` é chamada para salvar a lista de tarefas no `localStorage`.

  ### 2. Marcar Tarefa como Concluída ou Excluir
    <p align="center">
      <img src="https://github.com/user-attachments/assets/34b25bd0-15df-4a39-abcc-dec8a8ada05a" width="50%">
    </p>
- O evento de clique na lista `listContainer.addEventListener()` detecta interações com as tarefas. Caso o usuário clique no item de lista `li`, ele alterna a classe `checked` nesse item, isso serve para estilizar tarefas concluidas, no caso com um risco cortando as palavras da lista.
- Caso o usuário clicar no `span` "X", a tarefa é removida da lista.

  ### 3. Salvar Dados no localStorage
    <p align="center">
      <img src="https://github.com/user-attachments/assets/1ded0ba2-6836-4b95-8aba-ac9d267b5250" width="50%">
    </p>
- A função `saveData()` armazena o conteúdo HTML da lista de tarefas no `localStorage`, o que faz com que os dados não sejam perdidos, caso a página seja fechada ou recarregada.


  ### 4. Carregar Dados Salvos
    <p align="center">
      <img src="https://github.com/user-attachments/assets/962cf4ed-f976-444c-889a-350179485dd8" width="50%">
    </p>
- A função `showTask()` é chamada logo ao carregar o script. Ela recupera os dados armazenados no `localStorage` e os exibe na lista de tarefas, mas, somente se existirem dados salvos no `localStorage`.


<br>

## Funcionamento do app:
<p align="center">
  <img src="https://github.com/user-attachments/assets/59e0b2d8-7ac1-4f86-be83-91da51e1ecd7" width="80%">
</p>




















