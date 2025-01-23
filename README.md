# Projeto Desafio CT-MON: Solução Preditiva Baseada em Séries Temporais

Este projeto foi desenvolvido como parte do desafio proposto pelo Comitê Técnico de Monitoramento de Redes (CT-MON) da Rede Nacional de Pesquisas (RNP). O objetivo foi criar uma solução preditiva baseada em séries temporais para prever comportamentos futuros em redes computacionais, utilizando técnicas avançadas de mineração de dados.

## Organização do Projeto

O repositório está estruturado da seguinte maneira:

.
├── results/         # Resultados das previsões geradas pelo modelo
├── Test/        # Conjunto de teste
├── Train/       # Conjunto de treinamento
└── tf_Bf.ipynb      # Notebook principal com a implementação do pipeline
└── submission.csv     # Arquivo de submissão gerado com melhor resultado


## Principais Recursos do Projeto

- **Modelo Utilizado**: 
  - O modelo **Random Forest** foi ajustado e avaliado para prever comportamentos futuros, superando o baseline definido no desafio.
  
- **Pipeline de Pré-processamento**:
  - Agregação dos dados em janelas temporais.
  - Geração de estatísticas como *features*.
  - Normalização dos dados utilizando `MinMaxScaler`.

- **Otimização de Hiperparâmetros**: 
  - Realizada com `RandomizedSearchCV` para encontrar os melhores valores de forma eficiente.

- **Métrica Principal**: 
  - Mean Absolute Percentage Error (MAPE), com resultados superiores ao baseline.

## Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/luizznelson/proj-desafio_CT-MON.git
   ```
2. Navegue até o diretório do projeto:
   ```bash
   cd proj-desafio_CT-MON
   ```
3. Abra o notebook `tf_Bf.ipynb` para explorar ou executar o pipeline de solução:
   ```bash
   jupyter notebook tf_Bf.ipynb
   ```

## Resultados

- **Score no Kaggle**: `0.0830976647`, superando o baseline de `0.0995022123`.
- Os resultados detalhados estão organizados na pasta `results/`.

## Trabalhos Futuros

- Explorar redes neurais recorrentes como LSTM para capturar dependências temporais complexas.
- Integrar variáveis externas para enriquecer o modelo.
- Automatizar o pipeline de pré-processamento e seleção de modelos, tornando-o mais eficiente e escalável.

## Autores

**Arthur Sabino e Luiz Nelson**  
Desenvolvido para o desafio CT-MON como parte da disciplina de Tópicos em Redes - Mineração de Dados.

## Licença

Este projeto é de uso acadêmico e experimental. Consulte os autores para outros usos.
