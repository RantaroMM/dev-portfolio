---
title: "Gaugit (RID GAUG) — App Mobile com BLE para Dosímetro de Radiação"
date: 2026-03-01
authors:
  - me
summary: "Aplicativo mobile em React Native integrado a firmware embarcado via Bluetooth Low Energy (BLE) para transmissão em tempo real, espectroscopia de energia e configuração do detector."
tags:
  - Mobile
  - BLE & IoT
  - React Native
tech_stack:
  - React Native
  - Bluetooth Low Energy (BLE)
  - OpenDosimeter
  - Firmware Embarcado
  - Git
  - OpenAI Codex
  - Google Antigravity
featured: true
status: "Premiado · IPEN"
role: "Desenvolvedor de Aplicativo (Iniciação Científica)"
duration: "Mar 2026 – o momento"
---

O **Gaugit** (**RID GAUG**) é um aplicativo mobile em **React Native** desenvolvido na minha Iniciação Científica no **IPEN** (Butantã, São Paulo) para comunicação em tempo real com o firmware embarcado do **OpenDosimeter** via **Bluetooth Low Energy (BLE)**.

> **Reconhecimento:** Projeto premiado no **X Prêmio de Inovação Tecnológica do IPEN**.

## Visão Geral

O aplicativo conecta o hardware portátil de detecção de radiação ao smartphone, permitindo parear rapidamente com placas próximas, acompanhar contagens totais e taxas de contagem (CPS) em tempo real, inspecionar espectros de energia de 4096 canais e sincronizar parâmetros de segurança e compensação térmica diretamente com o detector.

O desenvolvimento contou com apoio de ferramentas de IA generativa (**OpenAI Codex** e **Google Antigravity**) para implementação, otimização e depuração de código, com versionamento em **Git**.

## Funcionalidades e Telas

### 1. Descoberta e Pareamento via BLE
Varredura de dispositivos BLE próximos exibindo nome e endereço MAC (como `Tupanexo`) para conexão direta com um toque.

![Tela de conexão BLE](screen-ble.png "Descoberta de dispositivos BLE próximos para pareamento")

### 2. Painel de Telemetria em Tempo Real (`RID GAUG`)
Exibe força de sinal BLE (`Strong` / `-68 dBm`), cronômetro da sessão, estado do equipamento (`IDLE`), **Total Counts**, **CPS** (contagens por segundo), **Live Time**, **Real Time** e botão central para iniciar/pausar a aquisição.

![Tela inicial de telemetria do Gaugit](screen-home.jpg "Dashboard principal com status de sinal, contagens, CPS e controle de aquisição")

### 3. Histograma Interativo de Espectro de Energia
Visualização em tempo real com **4096 bins**, modos de escala e zoom (`LOG`, `4X`, `FULL`), métricas resumidas (`Peak Ch`, `Total`, `CPS`, `Bins`) e tooltip interativo para inspeção de cada canal.

![Tela de histograma do Gaugit](screen-histogram.jpg "Histograma logarítmico de 1024 canais com inspeção detalhada por canal")

### 4. Configuração do Detector e Limites de Segurança
Ajuste de parâmetros enviados ao hardware (`Sync Board`), incluindo ativação de **Compensação de Temperatura**, **Breakdown Voltage (V)**, **Temperatura de Referência (°C)**, **Temp Factor (V/°C)**, **Overvoltage (V)**, cálculo de **Vbias** e seletor de tema (**System / Light / Dark**).

![Tela de configuração do detector no Gaugit](screen-setup.jpg "Configuração de tensão de polarização, compensação térmica e tema do app")

## Destaques Técnicos

- **Interface Mobile**: Construída em **React Native** com foco em legibilidade em campo e navegação em 4 abas (`Home`, `Histogram`, `Monitor`, `Setup`).
- **Comunicação BLE com Firmware**: Transmissão contínua de dados de radiação e sincronização bidirecional de parâmetros de operação com o **OpenDosimeter**.
- **Visualização Científica**: Plotagem logarítmica responsiva de 4096 canais com seleção interativa de picos e contagens.
