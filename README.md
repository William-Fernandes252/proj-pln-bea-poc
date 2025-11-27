# Bea - Brazilian Equity Analyzer

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/William-Fernandes252/proj-pln-bea-poc/blob/main/proj_pln_bea.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Descrição

**Bea** é um assistente financeiro inteligente especializado em análise de relatórios gerenciais de fundos de investimento e empresas listadas na B3. Este projeto foi desenvolvido como parte da disciplina de **Processamento de Linguagem Natural [2025-Q3]** na UFABC, ministrada pelo Prof. Alexandre Donizeti Alves.

O projeto utiliza o framework **LangChain** em conjunto com **Grandes Modelos de Linguagem (LLMs)** para aplicar técnicas de PLN em análise financeira.

## Técnicas de PLN Utilizadas

- **Sistemas de Perguntas e Respostas** (Question Answering)
- **Extração de Informações** de documentos financeiros
- **RAG (Retrieval-Augmented Generation)** para consultas em relatórios gerenciais

## Tecnologias

| Tecnologia | Descrição |
|------------|-----------|
| [LangChain](https://python.langchain.com/) | Framework para desenvolvimento de aplicações com LLMs |
| [OpenAI GPT-5 Nano](https://platform.openai.com/docs/models/gpt-5-nano) | Modelo de linguagem utilizado |
| [Tavily](https://tavily.com/) | API de busca para informações em tempo real |
| [FAISS](https://github.com/facebookresearch/faiss) | Vector store para RAG |
| [PyPDF](https://pypdf.readthedocs.io/) | Carregamento de documentos PDF |

## Funcionalidades

- 📊 **Análise de Relatórios Gerenciais**: Carrega e analisa relatórios em PDF de fundos de investimento
- 🔍 **Busca Inteligente**: Utiliza RAG para consultar informações específicas nos documentos
- 🌐 **Busca Web**: Integração com Tavily para obter informações atualizadas do mercado
- 💬 **Chat Interativo**: Interface conversacional com memória de contexto
- 📈 **Cotações de Ações**: Consulta de preços e informações de ativos da B3

## Como Usar

### Pré-requisitos

- Conta Google (para usar o Google Colab)
- Chave de API da OpenAI
- Chave de API do Tavily

### Execução

1. Clique no badge "Open In Colab" acima
2. Execute as células de instalação de dependências
3. Configure suas chaves de API quando solicitado
4. Monte seu Google Drive (para carregar os documentos PDF)
5. Execute as células restantes para inicializar o agente
6. Utilize a função `chat_loop()` para interagir com a Bea

### Exemplos de Perguntas

```
- Qual é o preço da CMIG3?
- Qual foi a rentabilidade do Maxi Renda FII no último mês?
- Quais são os principais ativos do fundo Kinea Rendimentos?
```

## Estrutura do Projeto

```
proj-pln-bea-poc/
├── proj_pln_bea.ipynb   # Notebook principal com a implementação
├── LICENSE              # Licença MIT
└── README.md            # Este arquivo
```

## Documentos Suportados

O projeto foi desenvolvido para analisar relatórios gerenciais de fundos de investimento imobiliário (FIIs), incluindo:

- Maxi Renda FII (MXRF11)
- Kinea Rendimentos FII
- Patria Log FII

## Equipe

| Nome | RA |
|------|-----|
| William Fernandes Dias | 11202020043 |

## Licença

Este projeto está licenciado sob a licença MIT - consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

## Referências

- [Documentação LangChain](https://python.langchain.com/docs/)
- [OpenAI API](https://platform.openai.com/docs/overview)
- [Tavily API](https://docs.tavily.com/)
