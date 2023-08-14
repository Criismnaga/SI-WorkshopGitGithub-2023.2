# Material Git e GitHub: do zero ao push

<h2>Começando pelo básico</h2>
<h3>Geralmente quando vamos começar um novo projeto precisamos iniciar ou clonar um repositorio</h3>
<dl>
  <dt>git init</dt>
  <dd>Transforma a pasta escolhida em um repositorio git</dd>
  <dt>git clone <i>"chave HTTP"</i> "NomeDaPastaQueVoceQuer" </dt>
  <dd>Clona um repositorio já existente</dd>
</dl>

<h3>Repositório criado, precisamos "puxar" mudanças, caso tenha alguma, no arquivo</h3>
<dl>
  <dt>git pull</dt>
  <dd>Caso haja qualquer alteração nos arquivos do repositório, serão puxadas para nosso computador</dd>
</dl>

<h3>Ok! Repositorio já está atualizado. Como faço para enviar as mudanças que fiz para o repositório?</h3>

> Nesse caso, vamos precisar de 3 comandos super simples
<dl>
  <dt>git add "nome do arquivo"</dt>
  <dd>Adiciona o arquivo ao nosso "setor de mudanças" que iremos enviar para o repositório na nuvem. (Aqui vai uma dica: se usar um . no nome do arquivo irá adicionar todos os arquivos alterados)</dd>
  <dt>git commit -m "mensagem do commit"</dt>
  <dd>O commit vai agrupar todos os arquivos que estão no nosso "setor de mudanças" e colocar um nome neles. (A mensagem do commit é muito importante para que outras pessoas possam entender do que se trata aquele commit)</dd>
  <dt>git push</dt>
  <dd>Envia seus commits para o repositório remoto.</dd>
</dl>

##
<h2>Configurações iniciais</h2>
<h3>Sempre que for configurar seu ambiente git em um novo computador é necessario fazer algumas configurações iniciais</h3>
<dl>
  <dt>git config --global --list</dt>
  <dd>Lista todas as configurações atuais</dd>
  <dt>git config --global user.name "seu nome"</dt>
  <dd>Para setar o nome do usuário</dd>
  <dt>git config --global user.email "seu email"</dt>
  <dd>Para setar o email do usuário. (O email da sua conta do github)</dd>
</dl>

##

<h2>Trabalhando com branchs</h2>
<h3>Branchs são como novas linhas do tempo onde é possivel alterar o código sem mexer na branch main</h3>
<dl>
  <dt>git checkout -b NomeDaNovaBranch</dt>
  <dd>Cria uma nova branch a partir da branch atual</dd>
  <dt>git checkout NomeDaBranch</dt>
  <dd>Troca para a branch escolhida</dd>
  <dt>git branch -D NomeDaBranch</dt>
  <dd>Apaga a branch escolhida</dd>
  
</dl>











