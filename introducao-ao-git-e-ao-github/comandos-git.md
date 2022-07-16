#  **Git**

### **ENCRIPTAÇÃO:**

openssl sha1 texto.txt → Passa o arquivo pelo sistema de encriptação SHA1 (40 chars)

BLOBS: Armazena metadados (tipo de objeto, tamanho do arquivo etc).
TREES: Apontam para blobs e também para outras árvores.
COMMITS: Apontam para árvores, para o commit anterior, para o autor e para a mensagem. Possui um “carimbo” de data e horário.

### **SISTEMAS DE AUTENTICAÇÃO:**
 
CHAVE SSH: Conexão segura e encriptada entre duas máquinas.
WINDOWS

ssh-keygen -t ed25519 C “e-mail” (gera a chave)
cat id_ed25519.pub (mostra a chave que foi criada)
eval $(ssh-agent -s) (gera um Agent pid)
ssh-add id_ed25519 (fornece a chave privada)
 
TOKEN DE ACESSO PESSOAL: Substitui o uso de senha por um Token que pode ter tempo de expiração pré-determinado.

Gerado no próprio Github e deve ser copiado e guardado em um local seguro, pois não poderá mais ser acessado.
Utiliza o link HTTPS para clonar repositórios.

### **COMANDOS BÁSICOS:**

cd “nome do diretório”/ → Seleciona um diretório

cd .. → Retorna ao diretório anterior

ls → Lista os arquivos no diretórios

ls -a → Mostra arquivos ocultos no diretório

pwd → Mostra o diretório onde você está  

mkdir → Cria um diretório dentro da pasta em que você está

mv “nome do arquivo” ./”nova pasta”/ → Move um arquivo para uma outra pasta
 
git init → Gera um repositório (Uma pasta oculta na qual estará o código)

git config--global user.email “e-mail” → Determina o e-mail do autor

git config --global user.name “username” → Determina o nickname do autor

git config --list → Lista as suas configurações do git

git config --global --unset “configuração que deseja alterar” → Altera uma config do git

git add * → Diz ao Git que você quer incluir atualizações a um arquivo no próximo commit

git commit -m “nome do commit” → Fornece ao Git a atualização do arquivo

git remote add origin “link do repositório no Github” → Vincula o diretório ao repositório

git remote -v → Lista o repositório do Github que está vinculado

git push origin main → “Empurra” o que você fez para o repositório no GitHub

git pull origin main → “Puxa” as versões alteradas, para que você analise e as integre

git clone “link do repositório no Github” → Clona o repositório diretamente da git bash
