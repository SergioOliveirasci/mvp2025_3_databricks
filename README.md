
#  Projeto MVP 3 — Pipeline de Dados em Nuvem com Databricks
### Pós-Graduação em Data Science & Analytics — PUC-Rio  
**Sprint: Engenharia de Dados**

---

##  Visão Geral do Projeto

Este projeto implementa um **Pipeline de Engenharia de Dados em Nuvem**, utilizando a plataforma **Databricks**, com o objetivo de analisar **avaliações de medicamentos** a partir de um dataset público.

O foco do MVP é demonstrar, de forma prática, a construção de um pipeline **end-to-end**, cobrindo todas as etapas do ciclo de vida do dado, desde a ingestão até a geração de insights analíticos, seguindo boas práticas de **Data Engineering**.

O projeto utiliza a arquitetura **Medallion (Bronze, Silver e Gold)**, com persistência em **Delta Lake**, validação de qualidade dos dados e análises orientadas a perguntas de negócio.

---
## 🎥 Vídeo de Documentação do Projeto

O projeto conta com um **vídeo de documentação**, no qual são apresentados o contexto do MVP,
a arquitetura do pipeline, a execução no Databricks e a explicação dos principais resultados obtidos.

👉 Assista ao vídeo completo aqui:  
https://youtu.be/F18ketjug4A

---

## 🧾 Instalação e Configuração do Databricks

Para fins de transparência técnica e reprodutibilidade, foi incluído no repositório
um documento em PDF contendo prints do processo de instalação, configuração e
integração do Databricks Community Edition com o GitHub.

👉 Acesse o PDF de instalação do Databricks aqui:
/docs/Instalacao_Databricks.pdf

---

##  Objetivos do Projeto

- Construir um pipeline de dados escalável em ambiente de nuvem;
- Implementar ingestão, transformação e modelagem analítica de dados;
- Garantir qualidade e consistência dos dados ao longo do pipeline;
- Responder perguntas de negócio relacionadas à avaliação de medicamentos;
- Demonstrar domínio prático de Engenharia de Dados com Databricks.

---

##  Tecnologiias Utilizadas

| Categoria | Tecnologia |
|--------|-----------|
| **Plataforma Cloud** | Databricks Community Edition |
| **Processamento** | Apache Spark (PySpark) |
| **Armazenamento** | Delta Lake |
| **Linguagem** | Python |
| **Versionamento** | GitHub |

---

##  Arquitetura do Pipeline

O pipeline segue o padrão **Medallion Architecture**, organizado em três camadas:

###  Camada Bronze
- Dados brutos ingeridos diretamente do arquivo CSV;
- Preservação da estrutura original do dataset;
- Garantia de rastreabilidade e reprocessamento.

###  Camada Silver
- Limpeza e padronização dos dados;
- Renomeação de colunas e normalização de campos textuais;
- Preparação dos dados para análise.

###  Camada Gold
- Dados agregados e modelados para consumo analítico;
- Criação de tabelas voltadas para responder perguntas de negócio;
- Redução do volume por meio de agregações (ex.: por fabricante).

---

##  Fonte dos Dados e Licenciamento

O dataset utilizado foi obtido na plataforma **Kaggle**, sendo disponibilizado sob **licença de uso público (open data)**.

✔ Uso permitido para fins acadêmicos e educacionais  
✔ Não contém dados pessoais sensíveis  
✔ Em conformidade com boas práticas éticas de uso de dados  

---

##  Perguntas de Negócio Respondidas

O projeto responde, entre outras, às seguintes perguntas:

1. Quais fabricantes possuem os medicamentos com melhores avaliações?
2. Existe relação entre o uso terapêutico e a avaliação positiva?
3. Medicamentos com mais efeitos colaterais tendem a ter piores avaliações?
4. Quais medicamentos apresentam maior percentual de avaliações excelentes?
5. As avaliações positivas estão concentradas em poucos fabricantes?

---

##  Qualidade dos Dados

Foram implementadas verificações de qualidade que incluem:

- Análise de valores nulos e campos vazios;
- Validação de faixas válidas para percentuais (0–100);
- Consistência da soma das avaliações;
- Identificação de duplicidades lógicas.

---

##  Estrutura do Repositório

```
📦 mvp2025-3-databricks
 ┣ 📜 MVP3_PUCRJ_2025_SERGIOOLIVEIRA.ipynb
 ┣ 📜 MVP3_Documentacao_Completa.md
 ┣ 📜 README.md
 ┣ 📂 docs
 ┃ ┗ 📜 Instalacao_Databricks.pdf
```

---

##  Como Executar o Projeto

1. Crie uma conta na **Databricks Community Edition**  
    https://www.databricks.com/try-databricks

2. Conecte seu GitHub ao Databricks:
   - User Settings → Git Integration
   - Utilize um Personal Access Token

3. Clone este repositório no Databricks (Repos)

4. Abra o notebook do MVP e execute as células sequencialmente.

---

##  Trabalhos Futuros

- Automação do pipeline com Databricks Workflows;
- Normalização semântica de campos textuais via NLP;
- Criação de dashboards interativos;
- Aplicação de métricas ponderadas por volume de avaliações;
- Integração com novas fontes de dados.

---

##  Autor

**Sérgio Oliveira**  
Aluno da Pós-Graduação em Data Science & Analytics — PUC-Rio  

---

##  Agradecimentos

Agradecimento ao curso de **Pós-Graduação em Data Science & Analytics da PUC-Rio**, aos professores da disciplina de Engenharia de Dados e aos recursos educacionais que possibilitaram o desenvolvimento deste projeto.
