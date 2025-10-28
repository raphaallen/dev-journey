# Permissões Avançadas no Linux (chmod, chown, umask)

Entender permissões é essencial para segurança e administração.

## Modelo simbólico e numérico
- Simbólico: `rwx` para usuário, grupo e outros (ex: `u+rwx,g+rx,o-r`)
- Numérico: soma dos bits (r=4, w=2, x=1).  
  - `755` → dono rwx (7), grupo r-x (5), outros r-x (5)
  - `644` → dono rw- (6), grupo r-- (4), outros r-- (4)

## Comandos úteis
- `ls -l` → mostra permissões
- `chmod 755 arquivo.sh` → define permissões numéricas
- `chmod u+x script.sh` → adiciona permissão de execução ao dono
- `chown usuario:grupo arquivo` → altera dono e grupo
- `chgrp grupo arquivo` → altera apenas o grupo

## Setuid, setgid e sticky bit
- `chmod u+s arquivo` → setuid: executa com permissões do dono do arquivo
- `chmod g+s pasta` → setgid: arquivos criados herdam grupo da pasta
- `chmod +t pasta` → sticky bit (ex: `/tmp`): só dono pode remover arquivos

## Exemplo prático
```bash
# Tornar um script executável apenas para o dono
chmod 700 meu_script.sh

# Mudar dono para 'rafa' e grupo para 'dev'
sudo chown rafa:dev projeto/
