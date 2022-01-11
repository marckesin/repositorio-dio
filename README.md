# Repositório do curso Git/Github

## Comandos úteis:

Iniciar um repositório:

```
git init
```

Move todos os arquivos para a área de stage:

**obs:** os arquivos inseridos dentro de .gitignore não serão considerados no commit

```
git add .
git add --all
```

Move apenas os arquivos modificados para a área de stage:

```
git add -u
```

Remove todos os arquivos da área de stage:

```
git rm --cached -r .
```

Executar um commit:

```
git commit -m "texto que identifica o commit"
```

Verifica o status dos arquivos:

```
git status
```

Verifica quais alterações foram feitas no arquivo especificado:

```
git diff <arquivo>
```

 Reverte as alterações feitas no arquivo para sua última versão:

```
git checkout <arquivo>
```

---



Reinicializa as configurações de usuário:

```
git config --unset user.name
```

Reinicializa as configurações de e-mail do usuário:

```
git config --unset user.email
```

Verifica várias configurações, entre elas, usuário e e-mail:

```
git config --list
```

---



Cria uma nova branch originada da branch "main":

```
git branch <nome da branch>
```

Altera para a branch criada (todas as edições, criações e alterações serão feitas nessa branch):

```
git checkout <nome da branch>
```

Altera para branch "main":

```
git checkout main
```

Realiza a junção (merge) de duas branchs:

```
git merge <nome da branch>
```

---



Deleta a branch localmente:

```
git branch -d <nome da branch>
```

Deleta a branch remotamente:

```
git push origin --delete <nome da branch remota>
```

---

Especifica para qual destino (GitHub, Bitbucket, etc.) serão empurrados os arquivos do repositório local:

```
git remote add origin(variável que recebe a URL) + url do repositorio criado no GitHub
```

Especifica a branch "main" como destino:

```
git branch -M main
```

"Empurra" os arquivos do repositório local para o repositório remoto:

```
git push -u origin main
```

"Puxa" arquivos do repositório remoto para repositório local:

```
git pull origin main
```

---



Defina um nome de usuário do git:

```
git config --global user.name "John Locke"
```

Conferir nome de usuário do git:

```
git config --global user.name
```

