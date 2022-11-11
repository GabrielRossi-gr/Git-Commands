#  🛑(em processo de desenvolvimento >> por favor reporte os erros no issues)
 
 ⭐️  Star o projeto  
 🐛 Encontrar e relatar issues

<img src="https://cdn.discordapp.com/attachments/819226289789075497/1029415491858604063/git_and_github_logo.png" width="273" height="75" /> 

<h2> 📚 Ementa</h2>

####  🔸1--> Iniciar Versionamento   
####  🔸2--> Comandos Basicos        
####  🔸3--> Git Branch              
####  🔸4--> Clonar Repositorios     
####  🔸5--> Git Stash               
####  🔸6--> Git Log                 
####  🔸7--> Git Reset                
####  🔸8--> Git Revert              
####  🔸9--> Chaves                  


# Iniciar Versionamento
```
echo "# NOME_DO_REPOSITORIO" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/LINK_DO_REPOSITORIO.git
git push -u origin main

git remote add origin https://github.com/LINK_DO_REPOSITORIO.git
git branch -M main                             
git push -u origin main
```
# Comandos Basicos:
```
    git add .                                  //adiciona todos os arquivos
        or
    git add <nomeDoArquivo>                    //adiciona arquivos especificos
    git commit -m <"nomeDoCommit">             //commitar
    git status                                 //ver status
    git push origin main                       //enviar commit para branch 'main' no GitHub
    git pull                                   //puxar arquivos do GitHub para sua maquina
```
# Git Branch:
```
    git branch                                   //ver branches 
    git checkout -b <nomeDaBranch>               //cria uma branch
    git checkout <nomeDaBranch>                  //navega para a branch 'nomeDaBranch'
    git branch -d <nomeDaBranch>                 //deletar branch 'nomeDaBranch'
    git branch -m <nomeAtual> <novoNome>         //mudar nome da branch
                 or
    git branch -m <novoNome>                     //mudar o nome quando vc esta na branch
    git merge <nomeDaBranch>                     //juntar as branches  
    git branch -M "main"                         //mudar branch para main
```
# Clonar Repositorios:
```
    git clone <git@github.LinkDoRepositorio.git>
    
```
# Git Stash:
```
    git stash save <"nomeDoStash">               //guardar conteudo de forma temporaria
    git stash list                               //ver a lista do stash, guardado em vetores
    git stash pop <indiceDoVetor>                //pegar conteúdo do stash de volta
    git stash clear                              //limpar stash
```
# Git Log:
```
    git log                                      //ver historico de commits
    git log --oneline                            //historico em uma linha 
    git log --graph                              //historico em formato de grafico    
```
# Git Reset:
```
    git reset <HEART~1>                          //voltar para ultimo commit HEART~2 HEART~3 
    git reset <id do commit>                     //passar o id do commit como parametro
```
# Git Revert:
```
    git revert <cha1>                            //voltar para o commit 
```

# Chaves
### Criar Chave ssh: Chave Publica:
```
    ssh-keygen -t ed25519 -c <SeuGmailDoGithub@gmail.com> 

    //a chave vai ser o 'arquivo.pub' 
    //chaveexemplo: feuawucnuaenvee5g58455g45gmail@gmail.com
```

### Inicializar ssh:
```
    eval $(ssh-agent -s)
```
### Adicionar Chave Privada:
```
    ssh-add <caminhoDaChavePRIVADA>            //colocar o caminho do diretorio da pasta
```
