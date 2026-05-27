# Guia de Redes de Computadores para Instituições Educacionais
## Visão Técnica e Objetiva para Usuários sem Conhecimento em Redes

# 1. O que é uma Rede de Computadores?

Uma rede de computadores é o conjunto de equipamentos interligados para compartilhar informações, acesso à Internet, sistemas acadêmicos, impressoras, arquivos e serviços corporativos.

### Exemplo em uma Instituição Educacional

```text
👨‍🏫 Professor
      │
💻 Computador
      │
🔀 Switch
      │
🛡️ Firewall
      │
🌐 Internet
      │
🏢 Servidores
      │
📚 Sistemas Acadêmicos
```

---

# 2. Estrutura Geral de uma Rede Corporativa Educacional

## Camada Física

| Ícone | Componente | Função |
|--------|------------|---------|
| 🖥️ | Computadores | Acesso dos usuários |
| 💻 | Notebooks | Mobilidade |
| 🖨️ | Impressoras | Impressão compartilhada |
| 📶 | Access Points | Rede sem fio |
| 🔌 | Cabeamento | Comunicação física |
| 🗄️ | Rack | Organização dos equipamentos |

---

## Camada de Rede

| Ícone | Equipamento | Função |
|--------|------------|---------|
| 🔀 | Switch | Conecta dispositivos locais |
| 🌐 | Roteador | Comunicação entre redes |
| 🛡️ | Firewall | Segurança e filtragem |
| 📡 | Access Point | Wi-Fi institucional |
| ⚖️ | Load Balancer | Distribuição de carga |

---

## Camada de Serviços

| Serviço | Função |
|----------|---------|
| DNS | Traduz nomes para IP |
| DHCP | Distribui IP automaticamente |
| Active Directory | Controle de usuários |
| Arquivos | Compartilhamento de documentos |
| Impressão | Gestão de impressoras |
| Proxy | Controle de navegação |
| VPN | Acesso remoto seguro |
| Banco de Dados | Sistemas acadêmicos e administrativos |

---

# 3. Categorias da Infraestrutura

## 3.1 Usuários

### 👨‍🎓 Alunos
- Laboratórios
- Biblioteca
- Wi-Fi acadêmico

### 👨‍🏫 Professores
- Sistemas educacionais
- Ambientes virtuais
- Compartilhamentos

### 👨‍💼 Administrativo
- ERP
- Financeiro
- RH
- Secretaria

---

## 3.2 Equipamentos

### Estações de Trabalho
- Windows 10/11
- Ubuntu Desktop
- Linux Mint

### Servidores

#### Microsoft Windows Server
- Active Directory
- DNS
- DHCP
- File Server
- Print Server

#### GNU/Linux

Distribuições comuns:

- Ubuntu Server
- Debian
- Rocky Linux
- AlmaLinux

Serviços:

- Apache
- Nginx
- Samba
- PostgreSQL
- MySQL/MariaDB
- Docker

---

# 4. Fluxo de Comunicação da Rede

## Exemplo: acesso ao portal acadêmico

```text
👨‍🎓 Usuário
      │
      ▼
💻 Computador
      │
      ▼
🔀 Switch
      │
      ▼
🛡️ Firewall
      │
      ▼
🌐 Internet
      │
      ▼
🏢 Servidor Web
      │
      ▼
🗄️ Banco de Dados
```

---

# 5. Principais Serviços de Rede

## DNS

### Função

Transforma:

```text
portal.escola.edu.br
```

em:

```text
10.10.20.50
```

Benefícios:

- Facilidade de acesso
- Padronização
- Redundância

---

## DHCP

Distribui automaticamente:

- Endereço IP
- Máscara
- Gateway
- DNS

Exemplo:

| Parâmetro | Valor |
|------------|--------|
| IP | 10.10.20.55 |
| Máscara | 255.255.255.0 |
| Gateway | 10.10.20.1 |
| DNS | 10.10.20.10 |

---

## Active Directory (Windows)

Centraliza:

- Usuários
- Senhas
- Computadores
- Políticas

Exemplos:

- Bloqueio de USB
- Instalação automática de softwares
- Políticas de segurança

---

## Samba (Linux)

Permite compartilhamento entre:

- Windows
- Linux
- macOS

Exemplo:

```text
\\arquivos\professores
```

---

# 6. Segmentação da Rede (VLANs)

Separação lógica para segurança.

| VLAN | Setor |
|--------|--------|
| 10 | Administrativo |
| 20 | Professores |
| 30 | Alunos |
| 40 | Laboratórios |
| 50 | Servidores |
| 60 | Wi-Fi Visitantes |

Exemplo:

```text
VLAN 10 → Financeiro
VLAN 20 → Docentes
VLAN 30 → Alunos
```

---

# 7. Segurança da Informação

## Controles Essenciais

| Controle | Objetivo |
|-----------|-----------|
| Firewall | Bloquear acessos indevidos |
| Antivírus | Detectar malware |
| MFA | Dupla autenticação |
| VPN | Acesso remoto seguro |
| Backup | Recuperação de dados |
| Logs | Auditoria |
| Monitoramento | Detecção de incidentes |

---

## Camadas de Segurança

```text
🌐 Internet
     │
🛡️ Firewall
     │
🔍 IDS/IPS
     │
🔐 Controle de Acesso
     │
🏢 Servidores
```

---

# 8. Monitoramento

Ferramentas comuns

## Microsoft

- Windows Admin Center
- Event Viewer
- Performance Monitor

## GNU/Linux

- Zabbix
- Grafana
- Prometheus
- Nagios

Monitorar:

- CPU
- Memória
- Disco
- Rede
- Disponibilidade

---

# 9. Backup e Recuperação

Estratégia 3-2-1

### 3 cópias
- Produção
- Backup local
- Backup externo

### 2 mídias diferentes
- Disco
- Nuvem

### 1 cópia externa

- Datacenter
- Cloud

---

# 10. Exemplo de Ambiente Pequeno

## Até 100 usuários

```text
Internet
   │
Firewall
   │
Switch
 ├── PCs
 ├── Impressoras
 ├── Wi-Fi
 └── Servidor
```

---

# 11. Exemplo de Ambiente Médio

## 100 a 1000 usuários

```text
Internet
    │
Firewall HA
    │
Core Switch
 ├── VLAN Administração
 ├── VLAN Professores
 ├── VLAN Alunos
 ├── VLAN Servidores
 └── Wi-Fi Corporativo
```

---

# 12. Exemplo de Ambiente Grande

## Acima de 1000 usuários

```text
Internet
     │
Firewall Cluster
     │
Core Datacenter
     │
───────────────
│             │
Campus A   Campus B
│             │
MPLS/VPN
│
Datacenter
│
Servidores
```

---

# 13. Boas Práticas com Microsoft Windows

## Estações

- Atualizações automáticas
- Antivírus corporativo
- BitLocker
- MFA
- Menor privilégio

## Servidores

- Active Directory organizado
- GPO padronizadas
- DNS redundante
- Backup frequente
- Auditoria habilitada

---

# 14. Boas Práticas com GNU/Linux

## Servidores

- Atualizações periódicas
- SSH seguro
- Firewall ativo (UFW/Firewalld)
- Logs centralizados
- Usuários sem privilégios administrativos

## Segurança

- Chaves SSH
- Fail2ban
- SELinux/AppArmor
- Backup automatizado

---

# 15. Resumo da Arquitetura

```text
👨‍🎓 Usuários
      │
💻 Computadores
      │
📶 Wi-Fi / 🔀 Switches
      │
🌐 Roteadores
      │
🛡️ Firewalls
      │
🏢 Servidores Windows/Linux
      │
🗄️ Banco de Dados
      │
☁️ Nuvem e Internet
```

---

# Conclusão

Uma rede corporativa educacional integra pessoas, equipamentos e serviços para fornecer conectividade, segurança, disponibilidade e acesso aos recursos acadêmicos e administrativos. O uso combinado de Microsoft Windows e GNU/Linux permite construir ambientes robustos, escaláveis e seguros, seguindo boas práticas de segmentação, monitoramento, backup e proteção da informação.
