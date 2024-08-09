# README - Documentação do codigo javascript - Cadastro.
Este projeto consiste em uma aplicação web simples para cadastro e gerenciamento de usuários. Ele permite ao usuário:

Cadastrar Usuários: Os usuários podem inserir um nome e adicioná-lo a uma lista utilizando um campo de texto e um botão de salvar.

Gerenciar a Lista de Usuários: A lista de usuários cadastrados é exibida em uma tabela dinâmica, onde é possível editar ou excluir cada nome diretamente.

Validação de Acesso: Existe uma funcionalidade de validação de acesso, onde o sistema verifica se os campos de login e senha foram preenchidos antes de permitir o redirecionamento para a página de cadastro.

![foto1](foto1.png)




Este projeto é uma aplicação simples de cadastro de usuários em JavaScript, HTML e CSS.

## Funções

### 1. `acessar()`

**Descrição:**  
Esta função valida o acesso do usuário, verificando se os campos de e-mail e senha foram preenchidos. Caso algum campo esteja vazio, uma mensagem de alerta é exibida. Se ambos os campos estiverem preenchidos, o usuário é redirecionado para a página `cadastro.html`.

**Parâmetros:**  
Nenhum.

**Fluxo:**  
- Obtém os valores dos campos de e-mail (`loginEmail`) e senha (`loginSenha`).
- Verifica se ambos os campos estão preenchidos.

- Exibe um alerta caso algum campo esteja vazio.

### 2. `salvarUser()`

**Descrição:**  
Esta função armazena o nome do usuário em um array (`dadosLista`). Após adicionar o nome, a lista de usuários é atualizada e o campo de entrada de nome é limpo. Se o campo de nome estiver vazio, um alerta é exibido.

**Parâmetros:**  
Nenhum.

**Fluxo:**  
- Obtém o valor do campo de entrada de nome (`nomeUser`).
- Verifica se o campo está preenchido.
- Adiciona o nome ao array `dadosLista`.
- Atualiza a tabela de usuários chamando a função `criaLista()`.
- Limpa o campo de entrada de nome.
- Exibe um alerta se o campo estiver vazio.

### 3. `criaLista()`

**Descrição:**  
Esta função cria ou atualiza a tabela de usuários na página. Ela percorre o array `dadosLista` e gera uma linha na tabela para cada usuário, com opções para editar ou excluir o nome.

**Parâmetros:**  
Nenhum.

**Fluxo:**  
- Inicializa a tabela com o cabeçalho "Nome Usuário" e "Ações".
- Percorre o array `dadosLista` e cria uma linha para cada usuário.
- Adiciona botões de "Editar" e "Excluir" em cada linha.

### 4. `editar(i)`

**Descrição:**  
Esta função permite editar o nome de um usuário na lista. Quando acionada, ela preenche o campo de entrada de nome com o nome selecionado e remove esse nome do array `dadosLista`.

**Parâmetros:**  
- `i`: Índice da linha da tabela que corresponde ao nome do usuário a ser editado.

**Fluxo:**  
- Preenche o campo de entrada de nome com o valor correspondente no array `dadosLista`.
- Remove o nome selecionado do array.

### 5. `excluir(i)`

**Descrição:**  
Esta função permite excluir um nome da lista de usuários. Quando acionada, ela remove o nome do array `dadosLista` e também remove a linha correspondente na tabela.

**Parâmetros:**  
- `i`: Índice da linha da tabela que corresponde ao nome do usuário a ser excluído.

**Fluxo:**  
- Remove o nome correspondente do array `dadosLista`.
- Exclui a linha correspondente na tabela.

---

# 🎮Tecnologias e Fontes Utilizadas:

HTML para a estrutura da página. 

CSS para estilização e layout da interface.

JavaScript para manipulação da lista de usuários e validação de acesso.
## 🚧 Fontes utilizadas
* [Mozilla](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form)- The Form Element.
* [Alura](https://www.alura.com.br/artigos/escrever-bom-readme)- Como Escrever um README Incrível no seu GitHub.
 
 # 💋AUTORES
 [<img loading="bia.jpg" src="bia.jpg" width=115><br><sub>Ana Beatriz Silva.</sub>](https://github.com/biasantorii) |
| :---:
