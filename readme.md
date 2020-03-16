# Minha "cola" de Git

"Quem não cola não sai da escola" não é verdade nem mentira, na verdade o ideal é sempre estudar, mesmo fora da escola, e a cola é mais que necessária para consultar, copiar e colar até aprender (se estiver na escola, não faça isso na prova!).

## Iniciando um diretório local com um novo *branch* atualizado de um diretório remoto

1. Na pasta local que deseja colocar o novo *branch*, *inicie o bash* e use o comando:

		git init

2. Vincule essa pasta local ao diretório remoto com o comando:

		git remote add origin git@github.com:nome-usuário/nome-repositório

3. Para ter certeza e listar os diretórios remotos:

		git remote show origin

4. Atualize o master local com o que estiver no remoto:

		git pull origin master

5. Crie uma nova *branch* cópia da master:

		git checkout -b nome-branch


## Passar alterações de *branch* local para remoto

1. Depois de gravar suas alterações na branch local:

		git push origin nome-branch

## Verificar estado das alterações locais

1. Use `status`:

		git status