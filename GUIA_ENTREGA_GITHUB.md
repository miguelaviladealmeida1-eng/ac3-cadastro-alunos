# Guia de publicação no GitHub — AC3

Este repositório guarda os códigos-fonte e a documentação do projeto. **O GitHub não executa sozinho o servidor Node.js nem fornece o MySQL**; portanto, o link do repositório é o link do código, não um endereço de aplicação em funcionamento.

## 1. Criar o repositório

1. Entre em https://github.com/new.
2. Em **Repository name**, use `ac3-cadastro-alunos`.
3. Escolha **Public** se o professor precisa abrir o link sem solicitar acesso.
4. Não marque a opção de adicionar README, `.gitignore` ou licença, pois estes arquivos já estão neste projeto.
5. Clique em **Create repository**.

## 2. Enviar os arquivos pelo navegador

1. Na página do repositório vazio, escolha **uploading an existing file**.
2. Extraia o ZIP do projeto no computador.
3. Entre na pasta `AC3_Fontes_do_Projeto` e selecione os arquivos e pastas do projeto, incluindo `public/`.
4. **Não envie `config.json`, senhas ou a pasta `node_modules/`.** O arquivo `config.json` é criado localmente a partir de `config.example.json`.
5. Escreva a mensagem `Adiciona projeto AC3 de cadastro de alunos` e confirme em **Commit changes**.

## 3. Link para o Forms

Depois do envio, copie o endereço principal do repositório, no formato:

`https://github.com/SEU_USUARIO/ac3-cadastro-alunos`

Abra o link em uma janela anônima para conferir se o professor consegue visualizar os arquivos.

## 4. Sobre a execução e a publicação

O projeto usa Node.js + Express no servidor e MySQL no banco. GitHub Pages não executa Node.js nem hospeda MySQL. Para demonstrar o sistema funcionando, é necessário executar o servidor com um MySQL disponível (conforme o README principal) ou contratar/configurar hospedagem compatível para os dois serviços.

O ambiente de execução descrito pelo professor continua sendo a referência da atividade. O repositório comprova a organização e disponibilização do código, mas não substitui as evidências reais de execução, operações CRUD e consulta SQL solicitadas.
