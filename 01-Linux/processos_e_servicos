
---

### 3) `01-Linux/06_processos_e_servicos.md`
```markdown
# Processos e Serviços (ps, top, systemctl)

Controlar processos é parte do dia a dia em servidores e dev.

## Listar processos
- `ps aux` → lista todos os processos
- `ps -ef` → alternativa com colunas diferentes
- `top` ou `htop` → monitoramento em tempo real (htop mais visual)
- `pgrep nome` → busca PID por nome

## Matar processos
- `kill PID` → SIGTERM (educado)
- `kill -9 PID` → SIGKILL (forçado)
- `pkill nome_processo` → mata por nome

## Serviços com systemd
- `systemctl status nome_servico` → ver status
- `sudo systemctl start nome_servico` → iniciar
- `sudo systemctl stop nome_servico` → parar
- `sudo systemctl restart nome_servico` → reiniciar
- `sudo systemctl enable nome_servico` → ativa no boot
- `sudo systemctl disable nome_servico` → desativa no boot

## Exemplo prático
```bash
# Verificar serviço nginx e reiniciar
systemctl status nginx
sudo systemctl restart nginx
