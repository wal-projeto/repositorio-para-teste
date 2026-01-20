"#repositorio-teste" 

criando um novo repositório atraves da linha de comando.


primeiro crio uma pasta no meu diretorio preferido, que nesse caso chamei de REPOSITORIO-TESTE , e abro aqui no
VSCode ela, depois abro um terminal estando nala e crio o arquivo readme.md atraves desse comando:
echo "# repositorio-teste" >> README.md 

git init 
digitamos esse comando para inicializar esse repositorio no git, depois desse comando podemos verificar que na 
pasta do repositorio aparecera outra chamada .git(arquivo que detem todas as configuraçoes na nossa maquina)

git add README.md 
com esse comando adicionamos o arquivo readme.md na area de stage para ser comitado no seguinte passo. Para adicionar
todos os arquivos de uma so vez digitamos-> git add .

git commit -m "primeiro commit" 
agora estamos comitando pela primeira vez e colocando um nome no commit. Aparecera essa mensagem :

[master (root-commit) 833f73f] primeiro commit adicionando o arq read.me
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

git branch -M main 
aqui ele diz que criemos uma branch chamada main. Para saber qual branch estamos, digitamos git status:
essa mensagem do terminal significa que estamos na nossa branch chamada master:
[master (root-commit) 833f73f] primeiro commit adicionando o arq read.me
 1 file changed, 1 insertion(+)
 create mode 100644 README.md


git remote add origin https://github.com/wal-projeto/repositorio-para-teste.git
com esse comando estamos linkando esse repositorio criado na maquina(repositorio-teste) com o repositorio remoto la do github atreves dessa URL que passamos acima


 git push -u origin main
 com esse comando carregamos os aquivos do repositorio da maquina para o repositorio do github(que no caso de momento e so o arquivo readme.md)
 APARECERA ESSA MENSAGEM:
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 250 bytes | 125.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/wal-projeto/repositorio-para-teste.git
 * [new branch]      master -> master

COM ISSO NOSSA PASTA FOI CARREGADA PARA O GITHUB