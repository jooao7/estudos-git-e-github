# 🔎 Resumos | Git e GitHub

Repositório para armazenar resumos sobre Git e GitHub

## Introdução ao Git

### O que é Git?

Git é uma ferramenta de controle de versão distribuída, essencial para a gestão de código fonte em projetos de desenvolvimento de software. Com ele, é possível manter um registro detalhado das alterações em arquivos, facilitando a colaboração entre desenvolvedores e permitindo o retorno a versões anteriores do código sempre que necessário.

## 📚 Documentação

- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/)

## 💻 Configuração Inicial do Git

Após a instalação do Git, é crucial configurar sua identificação e ambiente de trabalho. Comece definindo seu e-mail e nome de usuário, que serão utilizados para assinar suas alterações no código:

```
git config --global user.email "seuemail@example.com"
git config --global user.name "Seu Nome"
```

Defina também o editor de texto preferido para a resolução de conflitos:

```
git config --global core.editor "editor-name"
```

Por último, estabeleça o nome padrão da branch principal para novos repositórios:

```
git config --global init.defaultBranch "main"
```

Para verificar todas as configurações aplicadas, utilize:

```
git config --list
```

### ▶️ Criando um Repositório Git

Primeiro, crie um diretório para o seu projeto:

```
mkdir my-project
cd my-project
```

Dentro do diretório, inicialize o repositório Git:

```
git init
```

### 🗂️ Gerenciamento de Arquivos

Crie um arquivo e verifique o estado atual do seu repositório:

```
touch a.txt
echo "Initial content of a.txt" >> a.txt
git status
```

O comando git status mostra os arquivos não rastreados ou modificados. Para preparar o arquivo a.txt para um commit, use:

```
git add a.txt
git status
```

### 📝 Realizando Commits

Um commit é um registro de alterações feitas no repositório. Para criar um commit, execute:

```
git commit -m "Added a.txt with initial content"
```

Para visualizar o histórico de commits, utilize:

```
git log
```

### 👨‍💻 Trabalhando com Branches

Branches permitem desenvolver funcionalidades isoladamente sem afetar a branch principal, geralmente denominada main. Para listar, criar e alternar entre branches:

```
git branch
git branch new-feature
git checkout new-feature
```

Após desenvolver e testar sua funcionalidade na branch new-feature, você pode mesclar ela com a main:

```
git checkout main
git merge new-feature
```

Se a branch new-feature não for mais necessária, você pode excluí-la:

```
git branch -d new-feature
```

### 📋 Comandos Git Essenciais

Aqui está um resumo dos comandos Git mais utilizados:

    git init: Inicializa um novo repositório.
    git status: Exibe o estado atual do repositório.
    git add <file>: Adiciona arquivos ao próximo commit.
    git commit -m "message": Cria um commit com uma mensagem.
    git branch: Lista todas as branches.
    git checkout <branch>: Troca para a branch especificada.
    git merge <branch>: Integra mudanças de uma branch para outra.
    git branch -d <branch>: Deleta uma branch que foi mesclada.
    git branch -D <branch>: Força a exclusão de uma branch não mesclada.

Este guia básico oferece uma introdução ao uso do Git em seus projetos de software, cobrindo configuração, gerenciamento de arquivos e controle de versões com branches.

### Referências

- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/)
- [MDN Web Docs - Git and GitHub](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/GitHub)
