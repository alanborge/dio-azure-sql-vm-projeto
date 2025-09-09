# 🚀 Desafio de Projeto - Azure SQL + VM (DIO)

Este repositório contém a entrega do **Desafio de Projeto da DIO**: criação e configuração de recursos no **Microsoft Azure**, garantindo a comunicação entre uma **máquina virtual (VM)** e um **banco de dados SQL** por meio de **redes virtuais (VNets)** e **peering**.

---

## 📌 Objetivo
- Criar uma arquitetura no Azure que contenha:
  - Máquina Virtual (VM)
  - SQL Managed Instance (Banco de Dados)
  - Virtual Networks (VNets)
  - Peering entre VNets para comunicação segura

---

## 🔧 Passo a Passo Executado

1. **Criação de Resource Groups**
   - `myVM_group`
   - `AZ-900_Lab_DIO`

2. **Criação da Máquina Virtual (VM)**
   - Nome: `myVM`
   - Sistema Operacional: (informar qual usou, ex: Windows Server ou Ubuntu)
   - Configurado acesso via RDP/SSH

3. **Criação do Banco de Dados**
   - SQL Managed Instance: `sqlazure-2025`
   - Banco: `bancotesteazure`

4. **Configuração de Redes Virtuais**
   - `vnet-sqlazure-2025`
   - `vnet-brazilsouth`
   - `VNET1`

5. **Configuração de Peering**
   - Conexão entre `vnet-sqlazure-2025` ↔ `vnet-brazilsouth`
   - Status: ✅ *Connected / Fully Synchronized*

6. **Route Table**
   - Criada tabela de rotas `rt-sqlazure-2025` para direcionamento do tráfego

---

## 📸 Evidências
### Recursos criados no Azure
![Recursos Azure](./imagens/recursos-azure.png)

### Peering configurado
![Peering VNets](./imagens/peering-vnets.png)

---

## 🔗 Links Úteis
- [Documentação Azure Virtual Network Peering](https://learn.microsoft.com/pt-br/azure/virtual-network/virtual-network-peering-overview)
- [Documentação Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/)

---

## ✨ Próximos Passos (Evolução do Projeto)
- Criar tabelas no banco e popular com dados
- Conectar os dados ao **Grafana** ou **Power BI** para visualização
- Automatizar deploy com **Terraform ou Bicep**

---

## 📚 Autor
Projeto desenvolvido por **Alan Borges** durante o curso da [Digital Innovation One (DIO)](https://www.dio.me/).

