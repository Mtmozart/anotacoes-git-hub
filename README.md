### 🚀 Tecnologias Utilizadas

<div>
  <img src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</div>

---

## 🛠️ Comandos Git Essenciais

### Configuração Inicial

- **Configurar nome de usuário e email:**
  ```bash
  git config --global user.name "Seu Nome"
  git config --global user.email "seu.email@example.com"
  ```

### Gerenciamento de Repositórios

- **Criar um novo repositório:**
  ```bash
  git init
  ```

- **Clonar um repositório existente:**
  ```bash
  git clone <url-do-repositorio>
  ```

### Controle de Versão

- **Verificar o status dos arquivos:**
  ```bash
  git status
  ```

- **Adicionar arquivos para a área de stage:**
  ```bash
  git add <nome-do-arquivo>
  git add .
  ```

- **Fazer commit das alterações:**
  ```bash
  git commit -m "Mensagem descritiva do commit"
  ```

- **Visualizar o histórico de commits:**
  ```bash
  git log
  ```

### Gerenciamento de Branches

- **Criar uma nova branch:**
  ```bash
  git branch <nome-da-branch>
  ```

- **Mudar para outra branch:**
  ```bash
  git checkout <nome-da-branch>
  ```

- **Criar e mudar para uma nova branch:**
  ```bash
  git checkout -b <nome-da-branch>
  ```

- **Mesclar uma branch com a branch atual:**
  ```bash
  git merge <nome-da-branch>
  ```

- **Remover uma branch local:**
  ```bash
  git branch -d <nome-da-branch>
  ```

### Repositórios Remotos

- **Verificar repositórios remotos:**
  ```bash
  git remote -v
  ```

- **Adicionar um repositório remoto:**
  ```bash
  git remote add origin <url-do-repositorio>
  ```

- **Enviar commits para o repositório remoto:**
  ```bash
  git push origin <nome-da-branch>
  ```

- **Atualizar o repositório local com mudanças do remoto:**
  ```bash
  git pull origin <nome-da-branch>
  ```

### Revertendo e Desfazendo Alterações

- **Reverter mudanças locais:**
  ```bash
  git checkout -- <nome-do-arquivo>
  ```

- **Desfazer um commit específico (mantendo mudanças):**
  ```bash
  git reset --soft <id-do-commit>
  ```

- **Desfazer um commit específico (descartando mudanças):**
  ```bash
  git reset --hard <id-do-commit>
  ```

- **Restaurar para o último commit:**
  ```bash
  git restore .
  git checkout -- .
  ```

### Tags e Releases

- **Criar uma tag:**
  ```bash
  git tag <nome>
  ```

- **Enviar uma tag para o repositório remoto:**
  ```bash
  git push origin <nome-da-tag>
  ```

- **Remover uma tag:**
  ```bash
  git tag -d <nome>
  git push origin --delete <nome-da-tag>
  ```

- **Criar uma tag anotada com mensagem:**
  ```bash
  git tag -a <nome> -m "Mensagem da tag"
  ```

### Cherry-Picking

- **Reaproveitar commits de uma branch em outra:**
  ```bash
  git cherry-pick <hash-do-commit>
  ```

### Blame

- **Achar o autor de uma linha específica (use com cuidado):**
  ```bash
  git blame <arquivo>
  ```

### Submódulos no Git

Submódulos permitem incluir um repositório Git dentro de outro como um subdiretório. Isso é útil quando você deseja usar um projeto externo dentro do seu projeto, mantendo a habilidade de atualizá-lo separadamente.

#### Comandos Relacionados a Submódulos

- **Adicionar um submódulo:**
  ```bash
  git submodule add <url-do-repositorio> <caminho-opcional>
  ```

- **Inicializar submódulos em um repositório clonado:**
  ```bash
  git submodule update --init --recursive
  ```

- **Atualizar submódulos para o commit mais recente:**
  ```bash
  git submodule update --remote
  ```

- **Remover um submódulo:**
  ```bash
  git rm --cached <caminho-do-submodulo>
  rm -rf <caminho-do-submodulo>
  ```

- **Alterar a URL de um submódulo:**
  ```bash
  git config --file=.gitmodules submodule.<submodulo>.url <nova-url>
  git submodule sync <submodulo>
  git submodule update --init --recursive
  ```

#### Caso de Uso: Corrigindo Referências de Commits em Submódulos

1. Navegue até o diretório do submódulo:
   ```bash
   cd <caminho-do-submodulo>
   ```

2. Verifique o histórico do submódulo:
   ```bash
   git log --oneline
   ```

3. Resetar o submódulo para o commit correto:
   ```bash
   git checkout <hash-do-commit>
   ```

4. Volte ao diretório raiz do projeto:
   ```bash
   cd ..
   ```

5. Atualize o índice do repositório principal:
   ```bash
   git add <caminho-do-submodulo>
   ```

6. Commitar a alteração:
   ```bash
   git commit -m "Atualiza submódulo para o commit correto"
   ```

7. Push para o repositório remoto:
   ```bash
   git push origin <nome-da-branch>
   ```

### Comandos Avançados do Git

- **Visualizar commits de forma resumida:**
  ```bash
  git log --oneline
  ```

- **Exibir mudanças detalhadas entre commits:**
  ```bash
  git log -p
  ```

- **Visualizar o histórico de commits como um gráfico:**
  ```bash
  git log --graph
  ```

- **Customizar o formato de saída do log:**
  ```bash
  git log --format="%H %an"
  ```

- **Verificar diferenças entre commits específicos:**
  ```bash
  git diff <commit-antigo>..<commit-novo>
  ```

### O que é o `git stash`?

É um "armário temporário" onde você guarda alterações que ainda não estão prontas para commit, para poder limpar sua área de trabalho e mudar de branch, por exemplo.

---

### Comandos básicos do `git stash`

* **Guardar as mudanças (stashing):**

  ```bash
  git stash
  ```

  Isso guarda suas modificações (modificações em arquivos rastreados e também arquivos removidos) e limpa a working directory para o último commit.

* **Listar as stashes salvas:**

  ```bash
  git stash list
  ```

  Mostra todas as alterações guardadas, com nomes tipo `stash@{0}`, `stash@{1}`, etc.

* **Aplicar a stash mais recente (mas mantém ela salva):**

  ```bash
  git stash apply
  ```

  Aplica as mudanças guardadas, mas não remove da lista de stashes.

* **Aplicar e remover a stash mais recente:**

  ```bash
  git stash pop
  ```

  Aplica as mudanças guardadas e remove essa stash da lista.

* **Guardar uma stash com mensagem:**

  ```bash
  git stash save "Mensagem explicando a stash"
  ```

  Ou (a partir do Git 2.13, o `save` está depreciado, pode usar apenas `git stash push`):

  ```bash
  git stash push -m "Mensagem explicativa"
  ```

* **Guardar mudanças de arquivos específicos:**

  ```bash
  git stash push <arquivo1> <arquivo2>
  ```

* **Remover uma stash específica:**

  ```bash
  git stash drop stash@{1}
  ```

* **Limpar todas as stashes:**

  ```bash
  git stash clear
  ```

---

### Quando usar o `git stash`?

* Você começou a fazer alterações, mas precisa mudar para outra branch para consertar um bug urgente.
* Quer experimentar algo sem perder o que já fez até agora.
* Está com mudanças parciais que ainda não quer commitar.
