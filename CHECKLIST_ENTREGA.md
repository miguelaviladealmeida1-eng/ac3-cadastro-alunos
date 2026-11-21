# Checklist de validação e evidências da AC3

Use dados fictícios durante a demonstração.

- [ ] O banco `escola` e a tabela `alunos` foram criados no MySQL.
- [ ] A aplicação conectou ao MySQL e abriu em `http://localhost:3000`.
- [ ] A tela inicial exibiu os registros de exemplo.
- [ ] Um aluno fictício foi cadastrado e apareceu na tabela.
- [ ] O curso desse aluno foi alterado pela opção **Editar**.
- [ ] A página foi atualizada e o registro continuou salvo.
- [ ] O aluno de teste foi excluído e desapareceu da tabela.
- [ ] Campos vazios e e-mail inválido foram rejeitados.
- [ ] A consulta `SELECT * FROM escola.alunos;` foi executada no MySQL Workbench e conferida com a interface.
- [ ] Foram feitos prints reais da aplicação, do terminal e da consulta SQL.
- [ ] O repositório GitHub está público (se o professor precisa acessá-lo) e não contém `config.json`, senhas ou `node_modules/`.

## Evidências recomendadas

1. Tela inicial com os alunos de exemplo.
2. Cadastro de aluno fictício concluído.
3. Registro após a edição.
4. Lista após a exclusão.
5. Terminal mostrando o servidor conectado ao MySQL.
6. MySQL Workbench mostrando `SELECT * FROM escola.alunos;`.

Não use imagens simuladas como se fossem execução real. Se alguma etapa ainda não foi executada, deixe-a pendente até poder validá-la.
