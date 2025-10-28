# 🐧 Introdução ao Terminal Linux

O terminal é o coração do Linux.  
Dominar a linha de comando é o primeiro passo para se tornar um verdadeiro desenvolvedor e entender como o sistema operacional funciona.

---

## 🎯 Objetivo
Aprender os comandos básicos para navegar no sistema, manipular arquivos e entender a estrutura do Linux.

---

## 📂 Estrutura de Diretórios
Os diretórios principais do Linux seguem uma hierarquia bem definida:

| Diretório | Função principal |
|------------|------------------|
| `/home` | Onde ficam as pastas dos usuários |
| `/etc` | Arquivos de configuração do sistema |
| `/bin` | Comandos básicos do sistema |
| `/usr` | Aplicações e bibliotecas de usuários |
| `/var` | Logs e dados variáveis |
| `/root` | Diretório do usuário administrador (root) |

---

## 🧭 Navegação básica

| Comando | Função |
|----------|--------|
| `pwd` | Mostra o diretório atual |
| `ls` | Lista os arquivos e pastas |
| `cd nome_pasta` | Entra em uma pasta |
| `cd ..` | Volta um nível |
| `clear` | Limpa a tela |

📌 *Dica:* use `ls -la` para ver arquivos ocultos.

---

## 🛠️ Manipulação de arquivos

| Comando | Descrição |
|----------|-----------|
| `touch arquivo.txt` | Cria um arquivo vazio |
| `mkdir nova_pasta` | Cria uma nova pasta |
| `rm arquivo.txt` | Remove um arquivo |
| `rm -r pasta` | Remove uma pasta e seu conteúdo |
| `cp origem destino` | Copia arquivos |
| `mv origem destino` | Move ou renomeia arquivos |

---

## 💡 Dica bônus

Você pode combinar comandos com `&&`, por exemplo:

```bash
mkdir teste && cd teste && touch arquivo.txt && ls
👉 Isso cria uma pasta, entra nela, cria um arquivo e lista o conteúdo — tudo em uma linha!
