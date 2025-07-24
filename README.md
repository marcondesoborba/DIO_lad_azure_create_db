# ⚡ Início Rápido: Criar Instância Gerenciada de SQL do Azure

Este guia ensina como criar uma Instância Gerenciada de SQL do Azure usando o Portal do Azure. A Instância Gerenciada oferece alta compatibilidade com o SQL Server e é ideal para migração de bancos de dados locais para a nuvem.

## 🧾 Pré-requisitos

- Conta ativa no Azure
- Permissões adequadas (Contribuidor ou permissão `Microsoft.Sql/managedInstances/write`)
- Rede virtual/sub-rede configurada para Instância Gerenciada

## 🛠️ Etapas para Criar a Instância

1. **Acessar o Portal**
   - Entre no [Portal do Azure](https://portal.azure.com)
   - Vá para **SQL do Azure > + Criar > Instância Gerenciada de SQL**

2. **Configurar Informações Básicas**
   - Assinatura e grupo de recursos
   - Nome da instância e região
   - Autenticação: SQL (recomendado para início rápido)
   - Usuário administrador e senha (mínimo 16 caracteres)

3. **Computação e Armazenamento**
   - Camada de serviço: Uso Geral
   - Hardware: Standard Gen5
   - vCores e armazenamento conforme necessidade
   - Redundância de backup: geográfica (recomendada)

4. **Rede**
   - Selecionar rede virtual e sub-rede
   - Desabilitar ponto de extremidade público (recomendado para segurança)

5. **Segurança e Configurações Adicionais**
   - Manter configurações padrão para segurança
   - Definir ordenação, fuso horário e janela de manutenção
   - Adicionar marcações (ex: Proprietário, Ambiente)

6. **Revisar e Criar**
   - Verifique todas as configurações
   - Clique em **Criar** para iniciar a implantação

## 🗃️ Criar Banco de Dados

- Acesse a instância criada
- Clique em **+ Novo banco de dados**
- Escolha nome, fonte de dados e configurações adicionais
- Finalize com **Criar**

## 🔗 Conectar-se à Instância

- Copie o FQDN da instância na aba **Visão Geral**
- Use ferramentas como SSMS para conectar via SQL

## 📚 Recursos Adicionais

- [Documentação oficial](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart?view=azuresql&tabs=azure-portal)
- [Migração do SQL Server](https://learn.microsoft.com/pt-br/azure/azure-sql/migration-overview)
- [Configurar conectividade de VM](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/connectivity-architecture)

---

> 💡 Dica: Você pode testar gratuitamente por até 720 horas com uma instância de uso geral nos primeiros 12 meses.

