# Olá, sou o Felipe 👋

**Cloud Engineer · DevSecOps · SRE** — automação de infraestrutura, remediação de vulnerabilidades e confiabilidade
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

## ☁️ Referências de arquitetura multi-cloud

Documentação de referência — não extraída de produção, e sim pensada como ponto de partida replicável — cobrindo
rede, Kubernetes gerenciado e camadas de dados nas quatro nuvens lado a lado, cada uma com Terraform completo
e o passo a passo equivalente pelo console/portal.

| Repositório | O que faz |
|---|---|
| 🟧 [**Arquitetura-Kubernetes-AWS**](https://github.com/FelipeFranca07/Arquitetura-Kubernetes-AWS) | Rede, EKS e dados ponta a ponta na AWS — VPC, firewall, load balancer, Transit Gateway, RDS, S3 e DynamoDB. |
| 🔷 [**Arquitetura-Kubernetes-Azure**](https://github.com/FelipeFranca07/Arquitetura-Kubernetes-Azure) | Rede, AKS e dados ponta a ponta no Azure — VNet, NSG, Load Balancer, VNet Peering-Hub, Azure SQL, Blob Storage e Cosmos DB. |
| 🟢 [**Arquitetura-Kubernetes-GCP**](https://github.com/FelipeFranca07/Arquitetura-Kubernetes-GCP) | Rede, GKE e dados ponta a ponta no Google Cloud — VPC, firewall, Cloud Load Balancing, VPC Peering-Hub, Cloud SQL, GCS e Firestore. |
| 🔴 [**Arquitetura-Kubernetes-Huawei**](https://github.com/FelipeFranca07/Arquitetura-Kubernetes-Huawei) | Rede, CCE e dados ponta a ponta na Huawei Cloud — VPC, Security Group, ELB, Enterprise Router, RDS, OBS e GaussDB. |

## 🚢 Projeto de referência — CI/CD + GitOps

Também construído do zero para estudo/portfólio: demonstra, de ponta a ponta, o padrão de **GitOps com ArgoCD**
que times de plataforma usam hoje — o pipeline de CI nunca toca o cluster diretamente, ele só publica a imagem
e atualiza a *declaração* do estado desejado; quem aplica a mudança é sempre o ArgoCD, sincronizando a partir do Git.

| Repositório | O que faz |
|---|---|
| ⚙️ [**Nexus-Api**](https://github.com/FelipeFranca07/Nexus-Api) | API (FastAPI) com testes automatizados e pipeline de CI/CD (GitHub Actions, com equivalentes em Azure DevOps e GitLab CI) que builda, testa, publica a imagem no GHCR e atualiza o repositório GitOps automaticamente. |
| 🔄 [**Nexus-GitOps**](https://github.com/FelipeFranca07/Nexus-GitOps) | Manifests Kubernetes via Kustomize (overlays dev/staging/prod) e Applications do ArgoCD no padrão *App of Apps* — a fonte da verdade do estado desejado do cluster. |

## 🧱 Stack

![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat&logo=ansible&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=FF9900)
![Microsoft Azure](https://img.shields.io/badge/Microsoft_Azure-0089D6?style=flat&logo=microsoftazure&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=googlecloud&logoColor=white)
![Huawei Cloud](https://img.shields.io/badge/Huawei_Cloud-C7000B?style=flat&logo=huawei&logoColor=white)
![Azure Pipelines](https://img.shields.io/badge/Azure%20Pipelines-0078D7?style=flat&logo=azuredevops&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat&logo=azure-devops&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-25292E?style=flat)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat&logo=gitlab&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat&logo=argo&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat&logo=powershell&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Windows Server](https://img.shields.io/badge/Windows%20Server-0078D6?style=flat&logo=windows&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

## 📎 Sobre estes repositórios

> Os repositórios `Ansible-*` documentam um padrão de arquitetura real — a lógica e as decisões de design são
> genuínas, mas todo dado específico de ambiente (hostnames, IPs, tokens, domínios) foi substituído por exemplos
> fictícios antes da publicação. Já os repositórios `Arquitetura-Kubernetes-*` e `Nexus-*` são documentação de
> referência construída do zero para estudo/portfólio, não uma extração de ambiente real.
