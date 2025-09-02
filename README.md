# 📊 ReportFlow

**ReportFlow** é uma aplicação fullstack para gerenciamento de **pedidos de relatórios e análises de dados**.  
Usuários podem solicitar relatórios (ex: vendas mensais por região) e o sistema processa essas requisições usando **Python (Pandas/Analytics)**, **Kafka** para mensageria e **n8n** para automações (ex: envio de e-mails com relatórios prontos).  

---

## 🚀 Tecnologias

- **Frontend**: React (dashboard para criar e acompanhar pedidos)  
- **Backend API**: Java + Spring Boot (gerenciamento de usuários e pedidos)  
- **Data Processing**: Python (consultas ao banco e geração de relatórios)  
- **Mensageria**: Apache Kafka (intermediário entre serviços)  
- **Banco de Dados**: PostgreSQL (armazenamento dos pedidos e relatórios)  
- **Automação**: n8n (envio automático de relatórios por e-mail/Slack)  
- **Infra**: Docker Compose (ou Kubernetes futuramente)  

---

## 📌 Exemplo de Pedido

```json
{
  "pedido_id": 789,
  "usuario": "analista@empresa.com",
  "tipo_relatorio": "vendas_mensais",
  "parametros": {
    "mes": "2025-08",
    "regiao": "sudeste"
  },
  "status": "solicitado"
}
