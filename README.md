# Olá, sou o Felipe 👋

**Cloud Engineer· DevSecOps · SRE** — automação de infraestrutura, remediação de vulnerabilidades e confiabilidade
de sistemas em produção.

## 🧰 O que tem por aqui

Os repositórios abaixo são **padrões de arquitetura** extraídos de automações reais que mantenho em produção —
documentados do zero, com hostnames, IPs e credenciais substituídos por exemplos fictícios. A ideia não é só
mostrar código, é documentar o *porquê* de cada decisão de design o suficiente pra alguém recriar o padrão do
zero no próprio ambiente.

| Repositório | O que faz |
|---|---|
| 🩺 [**Ansible-Auto-Healing**](https://github.com/FelipeFranca07/Ansible-Auto-Healing) | Checagem contínua de serviços com correção automática (restart) e notificação inteligente — silêncio quando está tudo bem, aviso informativo quando corrige sozinho, escalonamento para um analista só quando falha de verdade. Mais um relatório de turno consolidado, 3×/dia. |
| 🔧 [**Ansible-Linux-Patch**](https://github.com/FelipeFranca07/Ansible-Linux-Patch) | Patch mensal de segurança em servidores Linux via Ansible/SSH, com blacklist de pacotes sensíveis e verificação pacote-a-pacote do que realmente aplicou. |
| 🪟 [**Ansible-Windows-Patch**](https://github.com/FelipeFranca07/Ansible-Windows-Patch) | Windows Update mensal orquestrado via Ansible/WinRM a partir de um agente **Linux** — sem precisar de WSUS/SCCM. |
| 🛡️ [**Ansible-Mitigation-VMDR-E-SCA**](https://github.com/FelipeFranca07/Ansible-Mitigation-VMDR-E-SCA) | Remediação de vulnerabilidades (Qualys VMDR/SCA) com guardrails proporcionais ao risco e rastreabilidade completa de QID/CVE até a ação que corrigiu. |

## 🧱 Stack

![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat&logo=ansible&logoColor=white)
![Azure Pipelines](https://img.shields.io/badge/Azure%20Pipelines-0078D7?style=flat&logo=azuredevops&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat&logo=powershell&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=flat&logo=windows&logoColor=white)

## 📎 Sobre estes repositórios

> Cada um documenta um padrão de arquitetura real — a lógica e as decisões de design são genuínas, mas todo
> dado específico de ambiente (hostnames, IPs, tokens, domínios) foi substituído por exemplos fictícios antes
> da publicação.
