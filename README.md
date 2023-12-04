![Logo github_0_push1](https://github.com/Criismnaga/SI-WorkshopGitGithub-2023.2/assets/114539692/fccf0649-bd3d-4653-8d02-af611fb074c3)

# Material Git e GitHub: do zero ao push

Esse repositório é um material de apoio do Workshop "Git e Github: do Zero ao Push" ministrado na Semana de Imersão 2023.2 da Cesar School em Recife-PE.

É possível conferir o conteúdo da palestra no link ao lado: [Slides da palestra](https://www.canva.com/design/DAFq4wix2Hw/0xtt40B6VSb9itnp6E8SSg/view?utm_content=DAFq4wix2Hw&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)

Em caso de dúvidas optem por conferir a documentação oficial do git. Pode parecer complexo no início mas é algo muito rotineiro na vida do desenvolvedor de software. Quanto antes se pegar o jeito com as documentações melhor:

Documentação oficial do git: [Git Docs](https://git-scm.com/doc)

Então vamos para a parte prática!

## 📁🐙Começando pelo básico

### Geralmente quando vamos começar um novo projeto precisamos iniciar ou clonar um repositorio

Transforma a pasta escolhida em um repositorio git

```bash
git init
```

Clona um repositorio já existente

```bash
git clone chave_HTTP NomeDaPastaQueVoceQuer
 ```

### Repositório criado, precisamos "puxar" mudanças, caso haja alguma, no arquivo

Caso haja qualquer alteração nos arquivos do repositório remoto, serão puxadas para nosso computador

```bash
git pull
```

### Ok! Repositorio já está atualizado. Como faço para enviar as mudanças que fiz para o repositório?

> Nesse caso, vamos precisar de 3 comandos super simples

Adiciona o arquivo ao nosso "setor de mudanças" (staging area) que iremos enviar para o repositório remoto. (**Aqui vai uma dica**: se usar um **.** no lugar do nome do arquivo irá adicionar todos os arquivos alterados)

```bash
git add nome_do_arquivo
```

O commit vai agrupar todos os arquivos que estão no nosso "setor de mudanças" e colocar um nome neles. (A mensagem do commit é muito importante para que outras pessoas possam entender do que se trata aquele commit)

```bash
git commit -m "mensagem do commit"
```

Envia seus commits para o repositório remoto.

```bash
    git push
```

Caso seja a primeira vez que você está enviando seus commits para o repositório remoto, será necessário usar o comando abaixo:

```bash
git push --set-upstream origin main
```

## ⚙️🛠️ Configurações iniciais

Sempre que for configurar seu ambiente git em um novo computador é necessario fazer algumas configurações iniciais. Abaixo segue uma lista com os comandos mais importantes:

Lista todas as configurações atuais

```bash
git config --global --list
```

Para setar seu nome do usuário

```bash
git config --global user.name "seu nome"
```

Para setar o email do usuário. (O email da sua conta do github)

```bash
git config --global user.email "seu email"
```

## 🌿🔀 Trabalhando com branchs

Branchs são como novas linhas do tempo onde é possivel alterar o código sem mexer na branch main. É muito útil para quando você quer testar algo novo sem alterar o código principal do projeto.

Cria uma nova branch a partir da branch atual

```bash
git checkout -b nome_da_nova_branch
```

Troca para a branch escolhida

```bash
git checkout nome_da_branch
```

Apaga a branch escolhida

```bash
git branch -D nome_da_branch
```

Mescla 2 branchs. Tendo a branch que você está como branch de destino e a
branch que você quer mesclar como branch de origem

```bash
git merge branch_de_origem
```

Lista todas as branchs

```bash
git branch
```

## 🛠️📝 Comandos úteis

Compara seu repositório local com o remoto e identifica quais as alterações que você fez

```bash
git status
```

Mostra as alterações linha a linha dos arquivos modificados e ainda não foram adicionados ao staging area. (OBS: Use **"q"** para sair do modo de visualização)

```bash
git diff
```

Existem também algumas variações do comando, por exemplo:

- Compara 2 branchs

```bash
git diff branch1 branch2
```

- Compara 2 commits

```bash
git diff commit_hash1 commit_hash2
```

- Em vez de mostrar as diferenças linha a linha mostra apenas o nome dos arquivos alterados. (pode ser usado em conjunto com as outras variações)

```bash
git diff --name-only
```

Remove todos os arquivos da área de preparação (staging area), permitindo que você repense quais alterações deseja incluir no próximo commit.

```bash
git reset HEAD
```

Descarta todas as alterações dos arquivos que foram alterados no seu repositório local, permitindo que você volte ao estado do último commit do repositório remoto. Você pode subustituir o nome do aquivo por . e isso acontecerá com todos os arquivos (OBS: Use com cuidado pois não tem como recuperar os arquivos depois)

```bash
git restore nomeDoArquivo
```

## 📝⌨️ Outras dicas

Ao utilizar o git é bem prático utilizar comandos de linha (command lines) do sistema operacional para criar pastas e arquivos e navegar por eles. Abaixo segue um link com um resumo direto ao ponto sobre esses comandos:

[Link Windows](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands/)
[Linux/Mac](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)

## 👥 Autores

Lucas Gabriel

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucasgdbs/)  [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LucasGdBS)

Cristina Matsunaga

[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cristina-matsunaga/) [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Criismnaga)
