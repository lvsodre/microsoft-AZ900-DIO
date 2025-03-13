# <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Microsoft_Azure.svg/1200px-Microsoft_Azure.svg.png" width="25" height="25"/> Introdução ao Microsoft Azure 

[![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com)
[![Licença](https://img.shields.io/badge/Licença-MIT-blue.svg)](LICENSE)
[![Curso](https://img.shields.io/badge/Módulo-Introdução-green.svg)]()

## 🔹 O que é o Microsoft Azure?

O Microsoft Azure é uma plataforma de computação em nuvem criada pela Microsoft para construir, testar, implantar e gerenciar aplicativos e serviços através de datacenters gerenciados pela Microsoft ao redor do mundo.

## 🚀 Primeiros Passos com o Azure

### 📝 Criando uma conta no Azure

Para começar a usar o Azure, é necessário criar uma conta:

1. Acesse o portal do Azure: [https://portal.azure.com](https://portal.azure.com)
2. Clique em "Criar uma conta gratuita"
3. Siga as instruções para criar sua conta Microsoft (ou use uma existente)
4. Forneça as informações de faturamento necessárias
5. Verifique sua identidade por telefone
6. Adicione um cartão de crédito para verificação (não será cobrado durante o período gratuito)

### 💰 Conta Gratuita do Azure

A conta gratuita do Azure oferece:
- Créditos gratuitos para usar em 30 dias
- Acesso a mais de 25 produtos sempre gratuitos
- Sem compromisso automático - você decide se quer continuar após o período gratuito

## 📚 Conceitos Fundamentais

### 💼 CapEx vs OpEx

**CapEx (Capital Expenditure):**
- Despesas iniciais em infraestrutura física
- Dedução do custo da compra ao longo do tempo
- Grandes investimentos antecipados

**OpEx (Operational Expenditure):**
- Despesas operacionais ou do consumo do serviço
- Dedução no mesmo ano da despesa
- Modelo de pagamento conforme o uso (pay-as-you-go)

Com o Azure, você passa de um modelo CapEx (compra de servidores físicos) para um modelo OpEx (pagamento pelo uso dos recursos em nuvem).

### ☁️ Modelos de Implantação de Nuvem

**Nuvem Pública:**
- Serviços oferecidos pela internet e disponíveis para qualquer pessoa que deseje comprá-los
- Recursos compartilhados entre múltiplos clientes
- Exemplo: Microsoft Azure, AWS, Google Cloud

**Nuvem Privada:**
- Recursos de computação usados exclusivamente por uma única empresa
- Pode estar localizada no datacenter da própria empresa ou hospedada por um provedor terceirizado
- Maior controle e privacidade

**Nuvem Híbrida:**
- Combinação de nuvem pública e privada
- Flexibilidade para escolher onde executar suas aplicações
- Integração entre ambientes locais e na nuvem

## ✨ Benefícios do Azure

- **Economia**: Pague apenas pelo que usar, sem grandes investimentos iniciais
- **Escalabilidade**: Aumente ou diminua recursos conforme a necessidade
- **Segurança**: Múltiplas camadas de proteção para seus dados
- **Alta disponibilidade**: SLAs (Acordos de Nível de Serviço) que garantem disponibilidade
- **Agilidade**: Implante recursos rapidamente sem precisar configurar hardware

## 📊 Aprofundamento em Escalabilidade, Confiabilidade e Disponibilidade

### 🔄 Escalabilidade
A escalabilidade no Azure permite ajustar recursos conforme a demanda:
- **Escalabilidade vertical**: Aumentar a capacidade de processamento (CPU/Memória)
- **Escalabilidade horizontal**: Adicionar mais instâncias dos recursos

### 🛡️ Confiabilidade e SLAs (Service Level Agreements)
Os SLAs do Azure definem os compromissos de disponibilidade e desempenho:

| Nível de Disponibilidade | Tempo de Inatividade Anual | Aplicações Típicas |
|--------------------------|----------------------------|-------------------|
| 99% | 3,65 dias | Aplicações não críticas |
| 99,9% | 8,76 horas | Aplicações internas |
| 99,99% | 52,56 minutos | Aplicações voltadas ao cliente |
| 99,999% | 5,26 minutos | Aplicações críticas para negócios |

### 💰 Considerações de Custo vs. Disponibilidade
- Quanto maior o nível de disponibilidade, maiores os custos (OpEx)
- Estratégias para otimizar custos:
  - Escolher o SLA adequado para cada aplicação
  - Usar zonas de disponibilidade para alta disponibilidade
  - Implementar arquiteturas resilientes apenas onde necessário

### ⚙️ Gerenciamento
O Azure oferece várias ferramentas para gerenciamento de recursos:
- **Azure Portal**: Interface visual baseada na web
- **Azure CLI**: Interface de linha de comando
- **Azure PowerShell**: Cmdlets para administração
- **Azure Resource Manager**: Modelo para implantação e gerenciamento

*Nota: O aumento da disponibilidade representa um modelo de custo OpEx típico, onde você paga mais por níveis mais altos de serviço conforme necessário.*

## 🏗️ Modelos de Serviço em Nuvem

O Azure oferece três modelos principais de serviços em nuvem, cada um com diferentes níveis de controle e responsabilidade:

### 🖥️ IaaS (Infrastructure as a Service)
- **O que é**: Infraestrutura de computação como um serviço
- **Você gerencia**: Sistemas operacionais, middleware, aplicativos, dados
- **Azure gerencia**: Servidores, armazenamento, rede, virtualização
- **Exemplos no Azure**: Máquinas Virtuais, Redes Virtuais, Discos
- **Quando usar**:
  - Migração "lift-and-shift" de workloads
  - Ambiente de teste e desenvolvimento
  - Aplicações que exigem controle total da infraestrutura

### 🧩 PaaS (Platform as a Service)
- **O que é**: Plataforma de desenvolvimento e implantação como um serviço
- **Você gerencia**: Aplicativos e dados
- **Azure gerencia**: Sistema operacional, middleware, runtime, infraestrutura
- **Exemplos no Azure**: App Service, Azure Functions, Logic Apps, SQL Database
- **Quando usar**:
  - Desenvolvimento rápido de aplicativos
  - Análise de dados ou business intelligence
  - Aplicações sem necessidade de gerenciar a infraestrutura subjacente

### 📱 SaaS (Software as a Service)
- **O que é**: Software pronto para uso entregue pela internet
- **Você gerencia**: Configuração e uso do software
- **Azure gerencia**: Todo o stack, incluindo aplicativos e dados
- **Exemplos no Azure**: Microsoft 365, Dynamics 365, Microsoft Teams
- **Quando usar**:
  - Aplicações padronizadas (email, CRM, etc.)
  - Aplicações que requerem acesso via web ou mobile
  - Projetos com recursos limitados para manutenção de software

### 📈 Comparação de Responsabilidades

| Recurso | On-premises | IaaS | PaaS | SaaS |
|---------|-------------|------|------|------|
| Aplicativos | Você | Você | Você | Azure |
| Dados | Você | Você | Você | Azure |
| Runtime | Você | Você | Azure | Azure |
| Middleware | Você | Você | Azure | Azure |
| Sistema Operacional | Você | Você | Azure | Azure |
| Virtualização | Você | Azure | Azure | Azure |
| Servidores | Você | Azure | Azure | Azure |
| Armazenamento | Você | Azure | Azure | Azure |
| Rede | Você | Azure | Azure | Azure |

## 🔜 Próximos Passos

À medida que você avança no aprendizado do Azure, poderá explorar:
- Serviços de computação (VMs, Kubernetes)
- Armazenamento em nuvem
- Bancos de dados
- Inteligência Artificial e Machine Learning
- DevOps e ferramentas de desenvolvimento

# Como Criar um Grupo de Recursos no Microsoft Azure

## O que é um Grupo de Recursos?
Um grupo de recursos no Azure é um contêiner lógico que armazena recursos relacionados para uma solução Azure. Todos os recursos devem estar em um grupo de recursos, e cada recurso só pode estar em um grupo por vez.

## Passos para Criar um Grupo de Recursos 📋

1. **Acesse o Portal Azure** 🖥️
   - Entre em [portal.azure.com](https://portal.azure.com) com suas credenciais

2. **Navegue até Grupos de Recursos** 📁
   - No menu lateral esquerdo, clique em "Grupos de recursos"
   - Ou use a barra de pesquisa superior e digite "grupos de recursos"

3. **Inicie a Criação** ➕
   - Clique no botão "Criar" ou "+ Adicionar"

4. **Configure o Grupo** ⚙️
   - Selecione sua assinatura Azure
   - Digite um nome único para o grupo de recursos
   - Escolha a região (datacenter) para armazenar seus metadados

5. **Revise e Crie** ✅
   - Verifique as informações fornecidas
   - Clique em "Revisar + criar" e depois em "Criar"

6. **Aguarde a Implantação** ⏱️
   - O processo de criação geralmente leva apenas alguns segundos

Uma vez criado, você pode começar a adicionar recursos como máquinas virtuais, contas de armazenamento e bancos de dados ao seu novo grupo de recursos.

## 📖 Recursos para Aprendizado

- [Documentação oficial do Azure](https://docs.microsoft.com/azure)
- [Microsoft Learn](https://docs.microsoft.com/learn/azure)
- [Centro de Arquitetura do Azure](https://docs.microsoft.com/azure/architecture)

---

*Este README é uma introdução básica e será expandido conforme avançamos no aprendizado do Azure.*

[![GitHub stars](https://img.shields.io/github/stars/seu-usuario/seu-repositorio?style=social)](https://github.com/seu-usuario/seu-repositorio)
[![GitHub forks](https://img.shields.io/github/forks/seu-usuario/seu-repositorio?style=social)](https://github.com/seu-usuario/seu-repositorio)
[![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow)]()
