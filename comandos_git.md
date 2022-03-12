# COMANDOS IMPORTANTES DO GIT

## Iniciar o git num novo repositório local
### Dentro do repositório rodar o comando:
_$ git init_
<br />
<br />

## Configurando de forma global email e usuário
_$ git config --global user.email "email@email.com"_
_$ git config --global user.name "meunomenogithub"_
<br />
<br />

## Clonar repositório com link
_$ git clone https://github.com/..._
<br />
<br />

## Clonar repositório usando SSH
_$ git clone git@github.com:..._
<br />
<br />

## _A primeira vez que for usar a chave, vai pedir para confirmar, basta digitar yes e dar enter_
<br />
<br />

## Mostrar estado do projeto
_$ git status_
<br />
<br />

## Enviar as modificações para o controle de versão localmente
_$ git add ._
## ou 
_$ git add -A_
<br />
<br />

## Fazer o commit - atualizar o versões dos arquivos e pastas
_$ git commit -m "Comentario sobre as atualizações feitas no projeto!"_
<br />
<br />

## Atualizar no Github com os commits
### **origin:**  repositório no Github; **master:** base local;
_$ git push origin master_
<br />
<br />

## Para "linkar" uma pasta local a um repositório
_$ git remote add origin_
<br />
<br />

## Para confirmar o repositório remoto
_$ git remote -v_ 
<br />
<br />

## Para criar uma nova branch
### A branch padrão é a **master**
_$ git checkout -b nomedabranch_

## Para exibir as branchs
### A branch selecionada estará com um * na frente!
_$ git branch_

## Para selecionar a branch
_$ git switch nome da branch_



## Conexão SSH com o Github
<br />
<br />

## => No Git Bash: <=
### Para gerar as chaves (pública e privada)
_$ ssh-keygen -t ed25519 -C email@email.com_
<br />
<br />

### Ele vai mostrar o local onde as chaves serão salvas e pede para apertar o Enter
### Vai pedir uma senha
### Vai pedir para repetir a senha
<br />
<br />

### Depois será necessário copiar o conteúdo da chave pública
_$ cat chave_publica.pub_
<br />
<br />
    
### Copia o conteudo da chave e vai para o Github
<br />
<br />


### => No Github: <=
### Menu do Perfil (foto no canto superior direito) => Settings => SSH and GPG keys
### Clica no botão Ne SSH Keys em SSH keys
<br />
<br />

### Em Tittle, colocar um nome de referência que saiba qual máquina está autorizada

### Em key, cola a chave copiada do Git Bash
<br />
<br />

### Clica em Add SSH key
### Irá pedir senha para confirmar
<br />
<br />

## => No Git Bash: <=
### Ativar o SSH
_$ eval $(ssh-agent -s)_
<br />
<br />

### Passar a chave privada para o SSH
_$ ssh-add id_ed25519_
<br />
<br />

### Vai pedir para digitar a senha que foi usada






