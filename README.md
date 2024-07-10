## Git & GitHub

Este guia tem como objetivo auxiliar você a entender e usar os conceitos básicos do Git e do GitHub, desde a configuração inicial até a criação de projetos colaborativos.

### O que é Git?

O Git é um sistema de controle de versão distribuído, ou seja, cada desenvolvedor possui uma cópia completa do histórico do projeto. Isso facilita o trabalho em equipe, pois permite que cada membro faça alterações em seu repositório local e as compartilhe com os outros membros da equipe.

### Configurando o Git

1. **Instalação:** Baixe e instale o Git para o seu sistema operacional: [https://git-scm.com/downloads](https://git-scm.com/downloads)
2. **Configurando o usuário:** Execute os seguintes comandos no terminal:
    ```bash
    git config --global user.name "Seu Nome"
    git config --global user.email "seu_email@example.com"
    ```
3. **Verificando a configuração:**
    ```bash
    git config --list
    ```

### Usando o Git

1. **Criando um repositório:**
    ```bash
    mkdir meu-projeto
    cd meu-projeto
    git init
    ```
2. **Adicionando arquivos ao repositório:**
    ```bash
    git add .  # Adiciona todos os arquivos
    git add nome_do_arquivo  # Adiciona um arquivo específico
    ```
3. **Criando um commit:**
    ```bash
    git commit -m "Mensagem descritiva da alteração"
    ```
4. **Visualizando o histórico de commits:**
    ```bash
    git log
    ```
5. **Desfazendo o último commit:**
    ```bash
    git revert HEAD
    ```


### Conectando seu Repositório Local ao GitHub

1. **No terminal, adicione o repositório remoto:**
    ```bash
    git remote add origin <URL_do_repositório>
    ```
2. **Envie suas alterações para o repositório remoto:**
    ```bash
    git push origin master
    ```

### Boas Práticas com Git

* **Commits pequenos e específicos:** Cada commit deve se concentrar em uma única funcionalidade ou correção.
* **Mensagens de commit descritivas:** Utilize mensagens claras e informativas que expliquem o propósito da alteração.
* **Utilize branches:** Crie branches para cada funcionalidade ou bug, facilitando a organização e o merge de alterações.
* **Crie um arquivo .gitignore:** Utilize esse arquivo para ignorar arquivos temporários ou irrelevantes que não devem ser adicionados ao repositório.

### Convenções de Commits

Para garantir a padronização e a clareza das mensagens de commit, siga as convenções do [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/):

* **Tipo:** `feat`, `fix`, `docs`, `refactor`, `style`, `test`, `chore`, `build`, `ci`
* **Sujeito:** Uma descrição concisa da alteração.

**Exemplo:**

```
feat(login): Adiciona suporte a login com Google
```

### Gerando um Arquivo .gitignore

Utilize o serviço [https://www.toptal.com/developers/gitignore/](https://www.toptal.com/developers/gitignore/) para gerar um arquivo .gitignore personalizado para o seu projeto, incluindo padrões para ignorar arquivos específicos de acordo com a linguagem de programação e o sistema operacional.

### Ferramentas de Visualização

* **GitHub Desktop:** [https://desktop.github.com/](https://desktop.github.com/)
* **GitKraken:** [https://www.gitkraken.com/](https://www.gitkraken.com/)
* **Sourcetree:** [https://www.atlassian.com/software/sourcetree](https://www.atlassian.com/software/sourcetree)

### Recursos Adicionais

* **Documentação do Git:** [https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)
* **GitHub Help:** [https://docs.github.com/](https://docs.github.com/)

### Dicas Extras

* **Utilize um editor de código com suporte a Git:** como VS Code, Sublime Text, Atom, etc.
* **Utilize aliases para comandos Git frequentes:** configure aliases no seu arquivo de configuração para tornar seus comandos mais rápidos e eficientes.
* **Participe de projetos open source:** contribua para projetos existentes no GitHub para praticar seus conhecimentos e colaborar com outros desenvolvedores.
