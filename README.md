# AC3 — Cadastro de alunos

Projeto acadêmico de CRUD (Create, Read, Update e Delete) desenvolvido com Node.js, Express e MySQL.

## Requisitos
- Node.js 22 ou superior
- MySQL Server
- npm

## Configuração
1. Execute `script.sql` no MySQL como administrador. O script cria o banco `escola`, a tabela `alunos`, dois registros de exemplo e o usuário de laboratório `cruduser`.
2. Copie `config.example.json` para `config.json` e informe a senha definida no SQL. Não publique `config.json`.
3. Instale e inicie:

```bash
npm ci
npm start
```

4. Abra http://localhost:3000 no navegador da máquina que executa o servidor.

## Operações CRUD
| Método | Rota | Ação |
| --- | --- | --- |
| GET | /alunos | Lista alunos |
| POST | /alunos | Cadastra aluno |
| PUT | /alunos/:id | Atualiza aluno |
| DELETE | /alunos/:id | Exclui aluno |

POST e PUT recebem JSON com `nome`, `email` e `curso`.

## Testes recomendados
Cadastre um aluno fictício, edite seus dados, atualize a página para confirmar persistência e exclua o registro de teste. Confira também os dados com `SELECT * FROM escola.alunos;`.

## Segurança e limitações
A aplicação é destinada a laboratório acadêmico e não possui autenticação. Use somente dados fictícios e não a exponha publicamente com dados reais. A conexão com o MySQL é feita pelo servidor; credenciais devem permanecer em `config.json`, que está no `.gitignore`.

## Estrutura
- `server.js`: API Express e conexão com MySQL.
- `script.sql`: banco, tabela e usuário de laboratório.
- `public/`: interface HTML, CSS e JavaScript.
- `config.example.json`: modelo de configuração.
- `GUIA_ENTREGA_GITHUB.md` e `CHECKLIST_ENTREGA.md`: orientação e validação.

**Importante:** o repositório contém o código-fonte. Para demonstrar a execução real, configure o MySQL e registre evidências próprias dos testes.
