## Chatbot Hospitalar Inteligente (RAG)

Projeto de portfólio em Inteligência Artificial aplicada à área hospitalar, utilizando
**Retrieval-Augmented Generation (RAG)** para responder dúvidas sobre protocolos e processos
hospitalares com base em documentos públicos.

**Este chatbot não realiza diagnóstico médico.**
Seu objetivo é exclusivamente **apoio informacional**.



## Objetivo

Demonstrar a aplicação prática de:
- NLP
- Embeddings
- Busca semântica
- LLMs
- Arquitetura RAG

em um contexto realista da área da saúde, respeitando limites éticos.



## Arquitetura

Pergunta do usuário
↓
Busca semântica (FAISS)
↓
Recuperação de trechos relevantes
↓
Prompt controlado + LLM
↓
Resposta baseada nos documentos



## Estrutura do Projeto
```text
chatbot-hospitalar-rag/
│
├── data/
│ └── documents/
│ ├── Manual de Biossegurança Hospitalar.pdf
│ ├── Protocolo de Triagem Hospitalar.pdf
│ └── Segurança do Paciente.pdf
│
├── faiss_index/
│ ├── index.faiss
│ └── index.pkl
│
├── notebooks/
│ ├── 01_ingestao.ipynb
│ ├── 02_indexacao.ipynb
│ └── 03_consulta.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```



## Fontes dos Documentos

Os documentos utilizados são públicos e foram obtidos de fontes oficiais:

- Manual de Biossegurança Hospitalar (EBSERH)  
  https://intranet.ebserh.gov.br/sites/default/files/produtos-de-conhecimento/2025-01/MN.CSB_.001%20Manual%20de%20Biosseguran%C3%A7a%20v.1_0.pdf

- Documento de Referência do Programa Nacional de Segurança do Paciente (Ministério da Saúde)  
  https://bvsms.saude.gov.br/bvs/publicacoes/documento_referencia_programa_nacional_seguranca.pdf

- Acolhimento e Classificação de Risco em Serviços de Urgência (Ministério da Saúde)  
  https://bvsms.saude.gov.br/bvs/publicacoes/acolhimento_classificaao_risco_servico_urgencia.pdf



## Limites Éticos e Responsabilidade

- O chatbot **não realiza diagnósticos médicos**
- Não substitui protocolos institucionais
- Não oferece recomendações clínicas personalizadas
- Utiliza apenas informações contidas nos documentos fornecidos
- Em caso de ausência de informação, informa explicitamente



## Tecnologias Utilizadas

- Python
- LangChain
- OpenAI Embeddings
- FAISS
- Jupyter Lab
- Anaconda



## Autor

Stephano Douglas Antunes

Projeto desenvolvido para fins educacionais e de portfólio.
