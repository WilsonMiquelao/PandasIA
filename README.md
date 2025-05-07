# Projeto Python IA: Score de Crédito de Clientes

## Descrição do Projeto
Este projeto foi desenvolvido para um banco com o objetivo de prever o score de crédito dos clientes, classificando-os em três categorias: "Ruim" (Poor), "OK" (Standard) ou "Bom" (Good). O modelo de Inteligência Artificial analisa diversas características dos clientes para determinar sua pontuação de crédito.

## Ferramentas e Tecnologias Utilizadas

### Bibliotecas Python
- **Pandas**: Utilizado para manipulação e análise dos dados, incluindo a leitura de arquivos CSV e transformação dos dados.
- **Scikit-learn (sklearn)**: Biblioteca essencial para machine learning, usada para:
  - Pré-processamento de dados (`LabelEncoder` para codificação de variáveis categóricas).
  - Divisão dos dados em conjuntos de treino e teste (`train_test_split`).
  - Implementação de modelos de classificação (`RandomForestClassifier` e `KNeighborsClassifier`).
  - Avaliação de desempenho dos modelos (`accuracy_score`).

### Modelos de Machine Learning
- **Random Forest Classifier**: Modelo baseado em árvores de decisão, escolhido por sua alta acurácia (83.04%) no conjunto de teste.
- **K-Nearest Neighbors (KNN)**: Modelo alternativo testado, com acurácia de 74.41%.

### Pré-processamento de Dados
- **LabelEncoder**: Transformação de variáveis categóricas (como profissão, mix de crédito e comportamento de pagamento) em valores numéricos para que os modelos pudessem processá-las.
- **Tratamento de Dados**: Verificação de tipos de dados e ajustes para garantir a consistência do dataset.

### Fluxo do Projeto
1. **Importação e Exploração dos Dados**: Leitura do arquivo CSV e análise inicial dos dados.
2. **Pré-processamento**: Codificação de variáveis categóricas e preparação dos dados para treinamento.
3. **Treinamento dos Modelos**: Implementação e treinamento dos modelos Random Forest e KNN.
4. **Avaliação**: Comparação da acurácia dos modelos para seleção do melhor (Random Forest).
5. **Previsão em Novos Dados**: Aplicação do modelo escolhido para prever o score de crédito de novos clientes.

### Arquivos do Projeto
- **clientes.csv**: Dataset principal contendo informações históricas dos clientes.
- **novos_clientes.csv**: Dataset com novos clientes para os quais o score de crédito foi previsto.
- **previsoesIA.ipynb**: Notebook Jupyter com o código completo do projeto, desde a importação dos dados até a previsão final.

## Como Executar o Projeto
1. Instale as dependências:
- pip install pandas scikit-learn
2. Execute o notebook Jupyter `previsoesIA.ipynb` para reproduzir todas as etapas do projeto.

## Resultados
O modelo Random Forest alcançou uma acurácia de 83.04%, sendo selecionado para prever o score de crédito dos novos clientes. Os resultados das previsões são exibidos no notebook e podem ser utilizados pelo banco para decisões estratégicas.
