
---

### 2) `01-Linux/gerenciamento_pacotes_apt.md`
```markdown
# Gerenciamento de Pacotes com APT (Debian/Ubuntu)

APT é o gerenciador de pacotes das distros baseadas em Debian/Ubuntu.

## Comandos básicos
- `sudo apt update` → atualiza lista de pacotes
- `sudo apt upgrade` → atualiza pacotes instalados
- `sudo apt install nome_pacote` → instala pacote
- `sudo apt remove nome_pacote` → remove pacote (mantém configs)
- `sudo apt purge nome_pacote` → remove pacote e configs
- `sudo apt autoremove` → remove dependências não usadas

## Procurando pacotes
- `apt search termo`
- `apt show nome_pacote` → informações sobre o pacote

## Boas práticas
- Sempre `apt update` antes de instalar.
- Use `apt upgrade` regularmente em ambientes dev; em produção, teste atualizações.

## Exemplo prático
```bash
sudo apt update

Só lembrando que...

Em outras distros (Fedora, Arch) use dnf, pacman etc. Aprender o gerenciador de pacotes da sua distro é essencial.
sudo apt install curl git -y
sudo apt autoremove -y
  
