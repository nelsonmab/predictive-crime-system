# Predictive Crime System

**Sistema preditivo de crimes com ML, GNN e dashboard interativo**  
Autor: **Nelson Oliveira de Almeida**  
Ano: 2025

---

## Descrição

Este projeto é um sistema de previsão de crimes baseado em aprendizado de máquina (RandomForest) e Deep Learning (GCN).  
Inclui dashboard interativo em React + Leaflet para visualização de mapas, heatmaps e células de incidência de crimes.  

Os dados podem ser públicos ou privados (com autorização), e são agregados por célula para preservar a privacidade.

---

## Funcionalidades

- Backend FastAPI para previsões e endpoints REST  
- Frontend React + Leaflet para visualização de mapas  
- Protótipo GNN (Graph Convolutional Network) para previsão avançada  
- Notebook baseline com dados sintéticos  
- Seed automático de dados sintéticos no PostGIS  

---

## Requisitos

- Docker e Docker Compose  
- Node.js e npm ou yarn  
- Python 3.10+  
- Git  

---

## Instalação e execução

1. **Clonar o repositório**

```bash
git clone https://github.com/nelsonmab/predictive-crime-system.git
cd predictive-crime-system

Subir todo o sistema via Docker Compose

docker-compose up --build


Backend FastAPI: http://localhost:8000

Frontend React: http://localhost:3000

Banco PostGIS: localhost:5432

O backend executa o seed automático populando o banco com dados sintéticos.

Notebook baseline (opcional)

jupyter notebook models/baseline.ipynb


Treina RandomForest em dados sintéticos

Visualiza heatmaps

Calcula métricas AUC-PR

Testar API

/health → retorna status do backend

/predict → retorna previsões de crimes

LGPD e boas práticas

Dados devem ser agregados por célula

Anonimização obrigatória de dados privados

Controle de acesso e logs recomendados

Licença

© 2025 Nelson Oliveira de Almeida
Todos os direitos reservados.

Para uso público, recomenda-se atribuir créditos ao autor.


