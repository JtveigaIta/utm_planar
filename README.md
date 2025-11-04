**🛰️ Desenvolvido para pesquisa, inovação e segurança na aviação não tripulada do Brasil.**  

# 📚 Créditos e Licenciamento

**Autor:** Jackson Tavares Veiga
**Instituição:** ITA / SAC / Projeto BR-UTM
**Ano:** 2025

# 🛩️ **Simulador PlanAr UTM**

O **PlanAr UTM** é um simulador de gerenciamento de tráfego aéreo não tripulado, inspirado na lógica do **UTM (Unmanned Traffic Management)** brasileiro. Ele nasce dentro do contexto do **Projeto PlaNAR – Planador Autônomo para Ressuprimento Logístico**, com integração de diferentes módulos de inteligência, replanejamento e falhas.

Seu propósito é oferecer uma arquitetura modular e extensível para estudos, testes operacionais e pesquisas acadêmicas relacionadas à aviação do futuro, com suporte a simulação de cenários complexos e interação entre provedores UTM, operadores, drones e autoridades.

---

## 🎯 **Objetivos Principais**

- Simular o ecossistema operacional do UTM brasileiro de forma fidedigna.
- Avaliar conflitos, desconflitos e separação entre aeronaves não tripuladas.
- Reproduzir a comunicação entre provedores UTM, DECEA/ANAC e operadores.
- Incluir falhas operacionais, replanejamento dinâmico e resposta automatizada.
- Gerar registros, relatórios de não conformidade e dados para aprendizado de máquina.
- Servir como ambiente modular (um “lego” de UTM), para colaboração acadêmica.

---

## 🧱 **Arquitetura de Módulos**

O simulador é composto por três principais sistemas integrados:

| Sigla | Nome | Função |
|-------|------|--------|
| **MRCF** | Mission Replanning and Control Framework | Replanejamento tático de missões, análise de rotas, resposta a falhas e reconfiguração dinâmica de aeronaves. |
| **MIRF** | Módulo de Injeção e Recuperação de Falhas | Emula falhas em drones, sensores, comunicação, provedores e avalia resiliência do sistema. |
| **PlanAr UTM** | Núcleo do simulador | Infraestrutura que integra provedores UTM, operadores, OIRs, drones, conflitos, registros e relatórios. |

---

## 🗂️ **Blocos Funcionais do Simulador**

Os cinco grandes blocos principais são:

1. **Cenários e Espaço Aéreo**
   - Modelagem 4D do espaço aéreo.
   - Zonas de operação, volumes de exclusão, áreas urbanas/rurais, meteorologia.
   - Definição de rotas, reservas de espaço (como SARPAS) e condições iniciais.

2. **Provedor UTM / Autorização / OIR**
   - Processamento de solicitações de voo.
   - Autorização, comunicação com DECEA, aplicação de regras e limites operacionais.
   - Monitoramento de provedores USS e registros de não conformidade.

3. **Operador / Drone / Operação**
   - Modelos de drones (asa fixa, rotativa, tamanhos, pesos).
   - Envio de planos de voo, telemetria, identificação remota, controle e autonomia.

4. **Conflito / Separação / Desconflito**
   - Identificação de conflitos horizontais e verticais.
   - Ajuste de rotas, altitudes, replanejamento automático.
   - Geração de dados para IA e análises de segurança.

5. **Registro / Relatórios / Dashboards**
   - Registro de eventos, falhas, tempos de resposta e não conformidades.
   - Dashboards 2D/3D, mapas em tempo real, simulações visuais e relatórios automáticos.

---

## 🛠️ **Objetos Principais do Sistema**

| Objeto | Responsabilidade |
|--------|-------------------|
| **Simulação** | Controle global do tempo, ciclo de execução, logs, modo real/acelerado. |
| **Cenário** | Zonas, volumes 3D, condições iniciais, parâmetros de voo e ambiente. |
| **ZonaOperacional / Volume3D** | Representação de áreas controladas, restritas ou temporárias. |
| **Drone** | Estado, modelo físico, sensores, bateria, telemetria e falhas. |
| **Operador** | Submissão de planos de voo, monitoramento e decisões humanas. |
| **ProvedorUTM** | Autoriza voos, monitora restrições, comunica-se com o DECEA e outros provedores. |
| **OIR** | Órgão de Informações de Risco: envia dados de incidentes, falhas ou emergências. |
| **Conflito** | Detecção de violação de separação, classificação e armazenamento. |
| **MRCF** | Altera trajetórias, realiza replanejamento tático e coordena resposta a eventos. |
| **MIRF** | Injeta falhas e avalia a resiliência do sistema ao erro. |
| **Registro** | Banco de dados de logs, eventos, autorizações e não conformidades. |

---

## 🚀 **Possibilidades de Expansão (Lego UTM)**

O simulador foi projetado para suportar futuras expansões como:

- **Tarifação de voo e penalidades**
- **Modelos de saturação e equidade de acesso ao espaço aéreo**
- **Modelos econômicos, sociais e indicadores de desempenho**
- **Integração com sistemas ADS-B / ABSL adaptados a drones**
- **Modelo de comunicação remota, rádio e identificação digital**
- **Cenários meteorológicos, terrenos 3D e espaço-tempo 4D**
- **Representação internacional e integração de múltiplos países**

---

## 📊 **Interfaces e Visualizações**

O sistema oferecerá:

- **Dashboards operacionais**
- **Mapas dinâmicos 2D/3D**
- **Visualização de drones em tempo real**
- **Alertas de conflito e falhas**
- **Relatórios automáticos de não conformidade (PDF/Excel)**
- **Simulações com time-lapse ou em tempo real**

---

## ✅ **Próximos Passos**

- [ ] Gerar diagramas UML dos blocos principais  
- [ ] Criar repositório com estrutura do simulador  
- [ ] Definir modelos de dados dos principais objetos  
- [ ] Implementar comunicação entre módulos MRCF ↔ Provedor ↔ Drone  

---

**🛰️ Desenvolvido para pesquisa, inovação e segurança na aviação não tripulada do Brasil.**  

# 📚 Créditos e Licenciamento

**Autor:** Jackson Tavares Veiga
**Instituição:** ITA / SAC / Projeto BR-UTM
**Ano:** 2025

O conteúdo deste repositório é de uso **acadêmico e educacional**, protegido por registro de propriedade intelectual.
Citações devem incluir o nome do autor e o título do trabalho.

> “Mission Replanning and Control Framework (MRCF)”
> *© 2025 Jackson Tavares Veiga. Todos os direitos reservados.*

---
## 📚 Referências

## 📖 Como Citar Este Trabalho

Se você utilizar ou referenciar este projeto em pesquisas, relatórios ou publicações acadêmicas, por favor cite da seguinte forma:

> **Jackson T. Veiga.** *Mission Replanning and Control Framework (MRCF): A Strategic Architecture for BVLOS Operations in UTM Environments (in proceeds).*  
> Aeronautics Institute of Technology (ITA), Department of Science and Space Technology (CTE), São José dos Campos, SP, Brazil, 2025.  
> 📧 jackson.veiga.101422@ga.ita.br

Ou, em formato **BibTeX**:

@inproceedings{veiga2025mrcf,
  author    = {Jackson T. Veiga},
  title     = {Mission Replanning and Control Framework (MRCF): A Strategic Architecture for BVLOS Operations in UTM Environments},
  booktitle = {Proceedings of the Aeronautics Institute of Technology (ITA), Department of Science and Space Technology (CTE)},
  year      = {2025},
  address   = {São José dos Campos, SP, Brazil},
  note      = {(in proceeds)},
  email     = {jackson.veiga.101422@ga.ita.br}
}

[2] J. T. Veiga, M. A. Pessoa, F. Junqueira, P. E. Miyagi, and D. J. dos Santos Filho,  
“A systematic modelling procedure to design agent-oriented control to coalition of capabilities—in the context of I4.0 as virtual assets (AAS),” *Computers*, vol. 10, no. 12, p. 161, 2021.  

[3] J. T. Veiga, “Proposta de um método para o controle de coalizão de recursos virtuais baseado em multi-agentes no contexto I4.0,” *Ph.D. dissertation*, Universidade de São Paulo, 2022.  

[4] J. T. Veiga, “An Open Framework for UAS Mission Replanning: From Intellectual Property to Collaborative Research,” in *Proceedings of the [Conference AIAA]*, 2025. (Versão Completa em Revisão)  

[5] F. L. S. D. Santos, “pyAutonomousAgent: An academic tool for modeling autonomous agent behaviors using behavior trees,” *JATM*, 2023. [Online]. Available: [https://www.scielo.br/j/jatm/a/fqNpVmY4RhchPsGQGdjpXVd/](https://www.scielo.br/j/jatm/a/fqNpVmY4RhchPsGQGdjpXVd/)

---

# 🛡️ Direitos Autorais e Propriedade Intelectual (Rodapé)

- **Propriedade Intelectual:** Arquitetura de Controle Multi-Agente para Replanejamento de Missões de VANTs  
- **Autor Registrado:** Jackson Tavares Veiga  
