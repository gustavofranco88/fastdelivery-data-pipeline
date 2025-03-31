# FastDelivery - Pipeline de Dados para Otimização de Logística  

**Objetivo:** Coletar, processar e analisar dados de entregas em tempo real para otimizar rotas e reduzir atrasos.  

## Arquitetura  
```mermaid  
graph LR  
  A[APIs de GPS/Clima] --> B[Google Cloud Storage]  
  B --> C[PySpark ETL]  
  C --> D[BigQuery]  
  D --> E[Airflow]  
  E --> F[Dashboard Power BI]  
