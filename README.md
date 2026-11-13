# Sistema de Biblioteca

Projeto didático em PHP e MySQL para gerenciar o acervo de uma biblioteca. O código inclui autenticação, cadastro de usuários e livros, consulta do estoque, pesquisa e controle de sessão.

## Tecnologias

- PHP
- MySQL
- HTML, CSS e JavaScript
- Bootstrap 5 em algumas telas

## Funcionalidades encontradas

- Login e logout.
- Cadastro e listagem de usuários.
- Cadastro e listagem de livros.
- Pesquisa por título, autor ou identificador.
- Controle de sessão e expiração por inatividade.
- Módulo adicional de cadastro em `sistema-cadastro/`.

## Como executar localmente

1. Tenha PHP, MySQL e uma extensão MySQL para PHP disponíveis.
2. Crie o banco e as tabelas esperadas pelo projeto, como `biblio_estoque`.
3. Ajuste a conexão em `conexao.php` para o seu ambiente local.
4. Na raiz do repositório, execute:

```bash
php -S localhost:8000
```

5. Acesse `http://localhost:8000`.

## Estrutura

- `index.php`: consulta simples do estoque.
- `lista_livros.php`: listagem e pesquisa de livros.
- `novo_livro.php` e `novo_usuario.php`: formulários de cadastro.
- `login.php`, `logout.php` e `testLogin.php`: fluxo de autenticação.
- `sistema-cadastro/`: outro exemplo de CRUD e autenticação.

## Aviso

Este é um projeto de estudo e contém padrões antigos de acesso ao banco. Antes de qualquer uso fora do ambiente didático, mova credenciais para variáveis de ambiente, use consultas preparadas, não exiba senhas e revise autenticação e validação.
