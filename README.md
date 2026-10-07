# NEXUS - Assistente Pessoal de IA Local-First

## Visão Geral

**NEXUS** é um assistente pessoal de inteligência artificial focado em **execução local**, privacidade e segurança. Diferente dos assistentes convencionais, NEXUS combina múltiplos agentes especializados, memória persistente e um sistema robusto de permissões para oferecer uma experiência de IA verdadeiramente pessoal e controlada.

## Objetivo do Projeto

NEXUS foi desenvolvido para:

- 🎯 **Assistência Local-First:** Executar modelos de IA localmente, eliminando dependências de serviços em nuvem para operações principais
- 🧠 **Inteligência Modular:** Utilizar agentes especializados para diferentes domínios (trabalho, RPG, fitness, etc.)
- 💾 **Memória Persistente:** Manter contexto de conversas e aprendizados anteriores
- 🔒 **Segurança e Privacidade:** Sistema de permissões granulares e controle total sobre dados
- 💰 **Gerenciamento de Custos:** Wallet integrada para controlar gastos com APIs e serviços externos
- ⚡ **Automações:** Suportar workflows e automações personalizadas
- 🌐 **Interface Web:** Interface futura via Streamlit para facilitar interação

## Arquitetura Planejada

```
nexus/
├── README.md                    # Documentação do projeto
├── requirements.txt             # Dependências Python
├── .gitignore                   # Arquivos ignorados pelo Git
├── app/                         # Aplicação principal
│   ├── __init__.py
│   ├── main.py                 # Ponto de entrada
│   └── ui.py                   # Interface web (Streamlit)
├── core/                        # Núcleo central
│   ├── __init__.py
│   ├── config.py               # Configurações centralizadas
│   ├── logger.py               # Sistema de logging
│   └── security.py             # Segurança e permissões
├── agents/                      # Agentes especializados
│   ├── __init__.py
│   ├── base_agent.py           # Classe abstrata para agentes
│   ├── router.py               # Roteador de requisições
│   ├── trabalho_agent.py       # Agente para tarefas profissionais
│   ├── rpg_agent.py            # Agente para RPG
│   └── musculacao_agent.py     # Agente para fitness
├── memory/                      # Memória persistente
│   ├── __init__.py
│   └── memory_manager.py       # Gerenciador de memória
├── wallet/                      # Gerenciamento de custos
│   ├── __init__.py
│   ├── wallet.py               # Wallet principal
│   └── transactions.py         # Histórico de transações
├── services/                    # Serviços externos
│   ├── __init__.py
│   ├── ollama_client.py        # Cliente Ollama (IA local)
│   ├── pdf_service.py          # Processamento de PDFs
│   ├── email_service.py        # Integração com email
│   └── telegram_service.py     # Integração com Telegram
├── utils/                       # Utilitários
│   ├── __init__.py
│   ├── validators.py           # Validadores
│   ├── file_utils.py           # Utilitários de arquivo
│   └── prompt_utils.py         # Utilitários de prompts
├── data/                        # Dados locais
│   ├── conversations/          # Histórico de conversas
│   ├── pdfs/                   # PDFs processados
│   └── wallet/                 # Dados de wallet
└── tests/                       # Testes
    ├── __init__.py
    └── test_wallet.py          # Testes da wallet
```

## Stack Tecnológico

- **Python 3.8+** - Linguagem principal
- **Ollama** - Execução de modelos de IA localmente
- **SQLite/PostgreSQL** - Persistência de dados
- **Streamlit** - Interface web futura
- **FastAPI** (opcional) - API REST

## Status

🚀 **Projeto em Desenvolvimento Inicial**

- [x] Repositório criado
- [ ] Estrutura base implementada
- [ ] Core e agentes especializados
- [ ] Sistema de memória
- [ ] Wallet integrada
- [ ] Interface web

---

**Desenvolvido por:** zellotop-hash  
**Licença:** A definir  
**Data de Criação:** Outubro de 2026
