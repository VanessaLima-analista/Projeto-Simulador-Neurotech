# Ecossistema Global de Startups: Mapeando o Sucesso

##  Projeto  
Este repositório contém um estudo sobre o **ecossistema global de startups**, utilizando o dataset público
[Global Startup Success Dataset (Kaggle)](https://www.kaggle.com/datasets/hamnakaleemds/global-startup-success-dataset).  

O objetivo é responder à questão:  
**Qual é o perfil de uma startup bem-sucedida?**  

##  Objetivo da Análise  
- Investigar se o volume de investimento (funding) está relacionado ao sucesso.  
- Avaliar a influência do **país de origem** e do **setor de atuação**.  
- Identificar padrões em perfis de startups por meio de clusterização.  

##  Metodologia  
A análise foi realizada em **Python (Colab)** e seguiu quatro etapas principais:  

1. **ETL** – limpeza, padronização e criação da coluna `status` (Operating / Acquired / IPO).  
2. **EDA** – análise exploratória com gráficos e estatísticas descritivas.  
3. **Teste de Hipóteses** – comparação do funding entre startups adquiridas e operacionais.  
4. **Modelagem (Clusterização)** – uso do algoritmo **KMeans** para segmentação em três perfis.  

##  Principais Insights  

### 1. Financiamento não garante sucesso  
- Correlação entre funding, receita e valuation foi quase nula (-0.014 a 0.009).  
- Teste T resultou em **p-valor = 0.3808** → sem diferença significativa entre startups adquiridas e operacionais.  
- **Conclusão:** o funding isolado não é determinante para o sucesso.  

### 2. Concentração geográfica e setorial  
- **Países líderes:** Alemanha, Brasil, Japão, Reino Unido e EUA.  
- **Setores em destaque:** Tech, Gaming, EdTech e Energy.  

### 3. Perfis de startups (clusterização)  
- **Cluster 1:** baixo funding e poucos funcionários.  
- **Cluster 2:** alto funding e muitos funcionários.  
- **Cluster 3:** perfil intermediário.  

### 4. Tecnologias e sucesso  
- **Mais usadas:** Java, Spring, Node.js, React.  
- **Associadas a maior score de sucesso:** C++, Machine Learning, Node.js, React.  

##  Recomendações  

- **Para Investidores:** funding isolado não é indicador confiável de sucesso. Avaliar também país, setor e stack tecnológico.  
- **Para Empreendedores:** foco em modelo de negócio sólido e sustentável. A localização e a escolha do stack tecnológico podem influenciar.  

##  Aprendizados  
- Hipóteses precisam ser validadas com estatística.  
- O sucesso de startups é **multifatorial**.  
- Técnicas de ETL, EDA, clusterização e testes estatísticos foram essenciais para identificar padrões.  

##  Referências  
- Dataset: *Global Startup Success Dataset (Kaggle)*  
- Bibliotecas: Python, Pandas, Matplotlib, Seaborn, Scikit-learn  
