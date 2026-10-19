# Lab 3 - Stack de Monitorizacao Containerizada com Terraform e Docker

Projeto de automacao e monitorizacao utilizando Terraform e Docker.

## Arquitetura da Solucao
- Nginx (meu-container-web): Servidor web na porta 8080.
- PostgreSQL (meu-container-db): Base de dados na porta 5432.
- cAdvisor (cadvisor): Metricas de containers na porta 8081.
- Prometheus (prometheus): Servidor de metricas na porta 9090.
- Grafana (grafana): Visualizacao grafica na porta 3000 (Painel cAdvisor ID 14282).

## Como Executar
chmod 777 prometheus.yml
terraform init
terraform apply -auto-approve

## Como Destruir
terraform destroy -auto-approve
