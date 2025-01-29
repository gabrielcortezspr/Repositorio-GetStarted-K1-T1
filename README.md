# Repositorio-GetStarted-K1-T1

# Comandos Básicos - Revisao

### Listar arquivos no diretório atual, um por linha:
ls -1

### Exibir o conteúdo de um arquivo:
cat "access.log"

### Exibir as últimas linhas de um arquivo:
tail -5 "access.log"

# Manipulação de Arquivos e Diretórios
### Criar um arquivo vazio:
touch "take-the-command-challenge"

### Criar diretórios (incluindo subdiretórios):
mkdir -p tmp/files

### Copiar um arquivo para um diretório:
cp "take-the-command-challenge" tmp/files

### Mover um arquivo para um diretório:
mv "take-the-command-challenge" tmp/files

### Criar um link simbólico:
ln -s tmp/files/take-the-command-challenge "take-the-command-challenge"

# Exclusão de Arquivos e Diretórios
### Deletar arquivos e diretórios recursivamente:
find . -delete

### Deletar arquivos com uma extensão específica:
find . -name "*.doc" -delete

# Filtragem e Busca
### Filtrar linhas de um arquivo que contêm uma string específica:
grep "GET" access.log

### Listar arquivos que contêm uma string específica:
grep -l "560" *

### Listar caminhos de arquivos que começam com um nome específico:
find . -name "access.log*"

### Filtrar linhas que contêm uma string em arquivos específicos:
find . -name "access.log*" | xargs grep "500"