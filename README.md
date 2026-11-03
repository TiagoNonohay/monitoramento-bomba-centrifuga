# Monitoramento de Bomba Centrífuga — Telemetria Inicial

![Gráfico de Vibração](monitoramento_vibracao.png)

## Objetivo do Projeto
Estudo de sinais industriais e fundamentos de Manutenção Preditiva aplicados a ativos rotativos (bomba centrífuga), visando a transição de dados brutos para análise de integridade mecânica e operacional.

## Variáveis Monitoradas
- **`temperatura_c`**: Temperatura de operação (°C).
- **`vibracao_mms_rms`**: Velocidade de vibração (mm/s RMS).
- **`pressao_bar`**: Pressão de descarga/processo (bar).
- **`estado`**: Estado operacional do ativo (`RUNNING` / `STOPPED`).
**<img width="986" height="788" alt="image" src="https://github.com/user-attachments/assets/d2e59098-1b1a-405d-a2b0-7b69cbf852c8" />
**


## Hipóteses Iniciais
1. Variações temporárias de vibração e temperatura durante o ciclo `RUNNING` podem indicar oscilações na carga do processo ou perturbações transitórias.
2. A queda brusca de pressão e vibração às 10:55 reflete a parada programada do equipamento (`STOPPED`).

## Limitações dos Dados
- **Dados Sintéticos:** Base gerada exclusivamente para fins didáticos de manipulação de séries temporais.
- **Ausência de Contexto Mecânico:** Não há dados de placas do equipamento, frequência de giro (RPM), tipo de rolamento ou curvas de desempenho (H-Q).
- **Incapacidade de Diagnóstico:** Os dados atuais **não** confirmam nem descartam falhas específicas (cavitação, desalinhamento ou desbalanceamento).
