# site---EDUSOUND
# 🎵 EduSound — Monitoramento Acústico Inteligente

> **Status do Projeto:** 🛠️ Em Desenvolvimento / Ambiente de Validação

O **EduSound** é um sistema de monitoramento acústico escolar desenvolvido com foco nas turmas do Terceirão (CID, CONT, INFO, RH, MKT, AI). O objetivo é coletar a amplitude das ondas sonoras dentro das salas de aula, processar os níveis de decibéis em tempo real através de um microcontrolador ESP32 e dar um feedback visual imediato ("Semáforo Acústico") para conscientizar alunos e professores sobre os impactos do ruído no ambiente de aprendizado.

---

## 🚀 Arquitetura Tecnológica

O projeto é dividido em três camadas principais:
1. **Hardware & Firmware:** ESP32 SoC, Sensor de Som Analógico (Microfone) e Atuador LED RGB (Semáforo Acústico).
2. **Nuvem & Armazenamento:** Integração de rede Wi-Fi via ESP32 para transmissão de dados estruturados para o Google Sheets via requisições HTTP.
3. **Análise de Dados:** Painel interativo criado no **Power BI** (`EDUSOUND_powerBI.pbix`) integrado diretamente ao site do projeto.

---

## 📊 Ambiente de Simulação e Modelagem de Dados

> ⚠️ **Nota de Engenharia:** Atualmente, o sistema está operando em **modo de calibração com dados simulados (sintéticos)**. Essa abordagem visa validar a integridade dos gráficos no Power BI e a resposta visual do site antes da implementação do hardware e da coleta definitiva em campo nas salas de aula.

### Parâmetros de Calibração do Semáforo:
* 🟢 **40dB – 55dB:** Ideal (Ambiente controlado)
* 🟡 **56dB – 70dB:** Atenção (Ruído moderado/conversas paralelas)
* 🔴 **71dB ou mais:** Crítico (Excesso acústico prejudicial à saúde cognitiva)

---

## 👥 Equipe
* **Emanuelly** — *Desenvolvimento de Firmware e Site*
* **Julia** — *Análise de Dados e Modelagem no Power BI*
* **Nikolas B.** — *Arquitetura de Hardware e Documentação*

---

## 💻 Como Rodar o Projeto Localmente

1. Clone o repositório:
   ```bash
   git clone -b development [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)