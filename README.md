# notepad git/github   (em processo de desenvolvimento)

# --------------------------------------------------
# criar chave ssh: CHAVE PUBLICA:
### ssh-keygen -t ed25519 -c SeuGmailDoGithub@gmail.com 
//a chave vai ser o 'arquivo.pub' 
//chaveexemplo:feuawucnuaenvee5g58455g45gmail@gmail.com

# --------------------------------------------------
# inicializar ssh:
### eval $(ssh-agent -s)

# --------------------------------------------------
# adicionar chave PRIVADA:
### ssh-add 'caminhoDaChavePRIVADA'

