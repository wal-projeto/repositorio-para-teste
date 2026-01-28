"#repositorio-teste" 
2 MANEIRAS MANEIRA DE CLONAR O REPOSITORIO DO GITHUB PARA A MAQUINA E ATUALIZAR-LO LA NO GIT:
<br>
criando um novo repositório atraves da "LINHA DE COMANDO" ABRINDO UM TERMINAL NO VSCODE.
<br>

primeiro crio uma pasta no meu diretorio preferido, que nesse caso chamei de REPOSITORIO-TESTE , e abro aqui no <br>
VSCode ela, depois abro um terminal estando nala e crio o arquivo readme.md atraves desse comando:
->>>  echo "# repositorio-teste" >> README.md <br>

Logo escrevo o comando:
->>> git init <br>
digitamos esse comando para inicializar esse repositorio no git, depois desse comando podemos verificar que na <br>
pasta do repositorio aparecera outra chamada".git "(arquivo que detem todas as configuraçoes na nossa maquina) <br>
<br>

Logo escrevemo o comando:
-->>>  git add README.md  ou  git add . <br>
com esse comando adicionamos o arquivo readme.md na area de stage para ser comitado no seguinte passo. Para adicionar
todos os arquivos de uma so vez digitamos-> git add .

<br>
Logo escrevemos :
-->>>  git commit -m "meu primeiro commit"  <br>
agora estamos comitando pela primeira vez e colocando um nome no commit. Aparecera essa mensagem :
<br>
[master (root-commit) 833f73f] primeiro commit adicionando o arq read.me
 1 file changed, 1 insertion(+)
 create mode 100644 README.md


<br>
lo escrevemos :
->>>>   git branch -M main  <br>
aqui ele diz que criemos uma branch chamada main. Para saber em qual branch estamos, digitamos git status:
essa mensagem do terminal significa que estamos na nossa branch chamada master:
<br>
[master (root-commit) 833f73f] primeiro commit adicionando o arq read.me
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

<br>

logo digitamos:
->>> git remote add origin https://github.com/wal-projeto/repositorio-para-teste.git (copiamos a https la no github)
<br> 
com esse comando estamos linkando esse repositorio local criado no computador(repositorio-teste) com o repositorio remoto la do github atreves dessa URL acima que pegamos la no GitHub em <>codigo -> Clone-> HTTPS


-->>> git push -u origin main<br>
 com esse comando carregamos os aquivos do repositorio da maquina para o repositorio do github(que de momento so tehno o arquivo readme.md)
 <br>
APARECERA ESSA MENSAGEM:
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 250 bytes | 125.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/wal-projeto/repositorio-para-teste.git
 * [new branch]      master -> master
<BR>

COM ISSO NOSSO REPOSTITORIO FOI CARREGADA PARA O GITHUB

<BR>

SE EU ESTIVER EM UM PROJETO COM MAIS PESSOAS LÁ NO GITHUB é IMPORTANTE ANTES DO PUSH, FAZER UM: 
->>> PULL ORIGIN MASTER

POIS ASSIM  ATUALIZAMOS O REPOSITORIO LOCAL COM AS ALTERACOES MAIS RECENTES DO REPOSITORIO REMOTO DO GITHUB . É <br> feito um fetch das atualizacoes no repositorio remoto e em seguida faz um merge com a branch atual do repositorio <br> local, incorporando as alteracoes realizadas pelos demais colaboradores.
APARECERA UMA MENSAGEM NO TERMINAL ASSIM:
* branch   master   -> FETCH_HEAD
Already up to date.
<br>

E DEPOIS JÁ POSSO FAZER O MEU (PUSH) E SUBIR AS MINHAS ALTERACOES NO PROJETO LA NO GITHUB<br>

<br> 



SEGUNDA MANEIRA DE CLONAR O REPOSITORIO DO GITHUB PARA A MAQUINA E ATUALIZAR-LO LA NO GIT:
<br>

UTILIZANDO O GIT BASH:

<BR>
- Primeiro crio um novo repositorio no GitHub, que nesse caso chamei de repositório-para-teste e selecione que ele
crie junto um arquivo README.MD (é um arquivo de documentacao padrao necessario para descrever sobre o repositorio)

-Abro o Git Bash dentro de uma pasta no windows onde quero clonar o repositorio remoto do github para dentro dela<br>
botao direito na pasta e clicamos em " Open Git Bash here", ou seja, ele abre o terminal do git dentro da pasta
- Para clonar o repositorio do GitHub para meu computador, dentro do terminal do Bash digito: 
->   git clone https://github.com/wal-projeto/repositorio-para-teste.git <br>

Para obter esse https, entro no repositorio repositório-para-teste la no github, em  <> codigo -> clone - copio o https que no caso é o https://github.com/wal-projeto/repositorio-para-teste.git e colo no prompt de comando do bash <br>

- Agora, se eu entrar na pasta no windows D:\curso PLATAFORMA DNS\FORMACAO ARQUITETO DE SOFTWARE ja poderei ver a pasta  "repositorio-para-teste" que é o repositorio remoto clonado. E dentro dela encontramos o aquivo .git com todas as configurações do git e o arquivo readme.md

OBS: posso fazer esse processo do git clone dentro do meu VSCode(abro um terminal, com o comando "cd entro na pasta
que desejo clonar) e depois git clone https://github.com/wal-projeto/repositorio-para-teste.git <br>, depois é só
abrir a pasta e ja terei acesso ao arquivo read.md

-agora ja posso fazer qualquer alteração no arquivo read.md do repositorio local e seguir com os comandos abaixo para atualizar o repositorio remoto do GitHub:

git add .
git commit -m "nome do comite" (pode ser que depois desse comando ele peça o git config --global user.email "" e o user.name)
git push origin main (com isso as alterações ja estarão no GitHub )
