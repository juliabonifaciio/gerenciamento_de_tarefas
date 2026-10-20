# Sistema de Gerenciamento de Tarefas

## Descrição do Projeto

O **Sistema de Gerenciamento de Tarefas** tem como objetivo oferecer uma solução simples e eficiente para o controle de atividades.  
A aplicação permite **cadastrar, listar, atualizar e remover tarefas**, garantindo a **persistência dos dados** por meio de armazenamento em arquivo.  

O sistema foi desenvolvido em **Python**, utilizando o conceito de **modularização**, separando as responsabilidades em diferentes módulos para melhorar a organização e a manutenibilidade do código.

---

## Funcionalidades

- **Cadastro de Tarefas:**  
  Permite criar novas tarefas informando:
  - Descrição  
  - Data de vencimento  
  - Status (Pendente, Em andamento, Concluída)

- **Listagem de Tarefas:**  
  Exibe todas as tarefas cadastradas, permitindo filtrar por:
  - Status  
  - Data de vencimento  

- **Atualização de Tarefas:**  
  Possibilita editar informações já cadastradas ou atualizar o status da tarefa.

- **Remoção de Tarefas:**  
  Exclui tarefas cadastradas do sistema.

- **Persistência de Dados:**  
  Os dados são armazenados em arquivo (`.json` ou `.txt`), garantindo que as informações sejam preservadas mesmo após o encerramento do programa.

---

## Estrutura do Projeto

### `tarefas.py`
Contém as funções responsáveis pelas operações principais do sistema:
- Cadastrar novas tarefas  
- Listar tarefas  
- Atualizar status e informações  
- Remover tarefas  

### `persistencia.py`
Gerencia o armazenamento de dados, permitindo salvar e carregar as tarefas a partir de arquivos locais.  
Pode utilizar formatos como **JSON** ou **CSV**, de acordo com a necessidade do projeto.

### `interface.py`
Fornece a camada de interação com o usuário.  
Pode ser implementada como:
- **Interface de Linha de Comando (CLI)** — menus textuais e interação via terminal.  
- **Interface Gráfica (GUI)** — utilizando bibliotecas como `Tkinter` ou `PySimpleGUI`.

### `main.py`
Arquivo principal que executa o sistema, realizando a integração entre os módulos e controlando o fluxo de execução da aplicação.
