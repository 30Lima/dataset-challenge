# 🚢 Joy Shipyard – Dataset de Interações com Chatbot

Projeto desenvolvido no contexto do programa **FIAP Corporate** em parceria com a **Porto Seguro**, com o objetivo de criar uma base estruturada de interações simuladas entre usuários e um **chatbot de suporte técnico**, voltado para diagnóstico de problemas mecânicos e compra de peças automotivas.

---

## 📌 Objetivo

Construir um **dataset limpo e organizado**, com registros completos dos fluxos de conversas dos usuários com o chatbot, a fim de:

- Identificar **padrões de comportamento**.
- Reconhecer **demandas frequentes** por tipo de problema ou produto.
- Suportar, futuramente, a aplicação de **modelos de agrupamento (ex: K-Means)** para obtenção de insights e segmentação de usuários.

---

## 🧩 Estrutura dos Dados

- Cada linha representa uma conversa simulada com o chatbot.
- Cada coluna representa uma etapa de menu:
  - `MENU PRINCIPAL`
  - Submenus como `MENU DE CURIOSIDADES`, `MENU DE ORÇAMENTO COM IA`, `MENU DE PEÇAS`, etc.
- As opções escolhidas são numeradas e registradas.
- Campos não preenchidos originalmente com `"-"` foram convertidos para `0` no pré-processamento.

### Exemplos de menus:
- **Problemas Mecânicos**: motor, freio, suspensão, direção hidráulica, etc.
- **Peças**: radiador, sensor, alternador, injeção eletrônica, etc.
- **CuriOSIDADES**: sobre a empresa, tecnologias, equipe, etc.

---

## 📋 Coleta e Pré-processamento

1. Interações foram **simuladas manualmente**, totalizando **100 fluxos de conversa**.
2. Cada conversa foi convertida em estrutura tabular com campos padronizados.
3. A coluna de rótulos (`RESPOSTAS DO FLUXO`) foi removida após análise.
4. Caracteres `"-"` foram substituídos por `0` para permitir análise quantitativa.
5. O dataset final foi exportado como `dataset_finalizado.csv`.

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Google Colab
- GitHub (armazenamento do dataset)

---

## 📁 Arquivos do Projeto

- `challenge.csv`: dataset original de conversas.
- `dataset_finalizado.csv`: versão limpa e pronta para análise.
- `ModeloIA.joblib`: reservado para etapas futuras de aplicação de IA.

---

## 🎯 Possíveis Extensões

- Aplicação de **K-Means** para descobrir agrupamentos de usuários com padrões similares.
- Visualização dos fluxos mais recorrentes em dashboards.
- Aprimoramento do chatbot com base em análise dos clusters.

---

## 🧑‍💻 Equipe de Desenvolvimento

Projeto desenvolvido por alunos FIAP:
- Leonardo P. Santos – RM 557541
- Pedro H. Lima Santos – RM 558243
- Vitor Gomes Martins – RM 558244

---

**FIAP 2024 – Corporate | Mont Clio para Porto Seguro**
