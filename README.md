
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="150" height="150" /> 

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
    git add <nomeDoArquivo>                    //adiciona arquivos especificos

    git commit -m <"nomeDoCommit">             //commitar
    git status                                 //ver status
    git push origin main                       //enviar commit para branch 'main' no GitHub
    git pull                                   //puxar arquivos do GitHub para sua maquina
    git fetch                                  //buscar todas as alterações da branch remota para a local
    git checkout -- .                          //remover alterações não adicionadas e não commitadas
```
# Git Branch:
```
    git branch                                   //ver branches
    git branch -a                                //ver branches remotas e locais
    git checkout -b <nomeDaBranch>               //cria uma branch
    git checkout <nomeDaBranch>                  //navega para a branch 'nomeDaBranch'
    git branch -d <nomeDaBranch>                 //deletar branch 'nomeDaBranch'

    git branch -m <nomeAtual> <novoNome>         //mudar nome da branch
    git branch -m <novoNome>                     //mudar o nome quando vc esta na branch

    git merge <nomeDaBranch>                     //juntar as branches  
    git branch -M "main"                         //mudar branch para main
    git push origin <nomeDaBranch>               //subir a nova branch para o GitHub
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
### Artigo Com Todas As Informações Chave SSH:
```
    https://docs.github.com/pt/authentication/connecting-to-github-with-ssh
```
<!--
    ### Criar Chave ssh: Chave Publica:
    ssh-keygen -t ed25519 -c <"SeuGmailDoGithub@gmail.com"> 
    //a chave vai ser o 'arquivo.pub' 
    //chaveexemplo: feuawucnuaenvee5g58455g45gmail@gmail.com
-->
<!-- 
### Inicializar ssh:
```
    eval $(ssh-agent -s)
```
### Adicionar Chave Privada:
```
    ssh-add <caminhoDaChavePRIVADA>            //colocar o caminho do diretorio da pasta
```   

-----------------------
-->


### Gerar chave
```
   ssh-keygen -t rsa -b 4096 -C "seu_email@example.com"
```

### Ativar gerenciador de chaves
```
   eval "$(ssh-agent -s)"
```

### Adicionar a chave
```
   ssh-add ~/.ssh/id_rsa
```

### Copiar chave 
```
   pbcopy < ~/.ssh/id_rsa.pub            //mac
   cat ~/.ssh/id_rsa.pub                 //outro
   xclip -sel clip < ~/.ssh/id_rsa.pub   //linux
```

### Name config
```
   git config --global user.name "Seu Nome"
```

### Email config
```
   git config --global user.email "seu_email@example.com"
```











