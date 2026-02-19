# TelecomAgent 🛠️

**Agente IA Multi-Agente Autônomo para Troubleshooting de Redes FTTH/GPON**

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![CrewAI](https://img.shields.io/badge/CrewAI-0.51+-FF6F61)](https://www.crewai.com)
[![LangChain](https://img.shields.io/badge/LangChain-0.2+-32CD32)](https://python.langchain.com)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.38+-FF4B4B?logo=streamlit)](https://streamlit.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

### O que é?
Um **agente inteligente multi-agente** criado por um engenheiro de Telecom com +17 anos de experiência que transforma logs de erro (GPON, OLT, ONU, BGP, OSPF, etc.) em **passos de troubleshooting claros, comandos prontos e solução automática**.

Desenvolvido por **Alan Kardec Moreira** – Data Scientist & AI Engineer | Fundador da AM Consultoria.

### Por que isso muda o jogo para ISPs?
- Reduz tempo de análise de horas → minutos
- Usa **sua própria base de conhecimento** (manuais Huawei, Cisco, Mikrotik – RAG privado)
- 100% offline com Ollama ou rápido com Groq/Llama3.1
- Interface bonita no Streamlit + mapa de calor de falhas
- Fácil de implantar no cliente

### Funcionalidades (v1.0)
- ✅ Análise automática de logs
- ✅ RAG com manuais oficiais de equipamentos
- ✅ 4 agentes especializados (Analyzer, RAG Expert, Troubleshooter, Validator)
- ✅ Sugestão de comandos copiáveis
- ✅ Mapa de calor de falhas (Folium)
- ✅ Histórico em SQLite
- ✅ Deploy gratuito (Streamlit Cloud / Railway)

### Tech Stack
- **Core**: Python 3.11+, CrewAI, LangGraph, LangChain
- **LLM**: Ollama (Llama3.1 70B ou 8B) ou Groq
- **Vector DB**: ChromaDB
- **Frontend**: Streamlit
- **Visualização**: Folium, Pandas, Matplotlib
- **Banco**: SQLite
- **Deploy**: Docker (em breve)

### Como rodar localmente (em 3 minutos)

```bash
git clone https://github.com/alankardecm/TelecomAgent.git
cd TelecomAgent
pip install -r requirements.txt
streamlit run app.py
