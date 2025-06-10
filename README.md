
1. Introdução
A rotatividade de clientes, chamada de “churn”, é um desafio importante para empresas de telecomunicação. Por meio da análise dos registros de clientes, é possível construir modelos preditivos que antecipem quais consumidores têm maior probabilidade de cancelar seus serviços. Isso permite à empresa direcionar estratégias específicas para retenção.

No cenário deste estudo, buscamos identificar fatores que influenciam o abandono e criar um modelo eficiente para prever a saída de clientes.

2. Sobre os Dados
O conjunto de dados utilizado está disponível no Kaggle.

Total de registros: 7043
Número de variáveis (preditoras): 20
A variável de interesse é: Churn

Entendendo o Dataset
Indica quais clientes cancelaram no último mês (coluna Churn).
Lista de serviços contratados: telefone, múltiplas linhas, internet, recursos de segurança, backup, suporte técnico, streaming, etc.
Informações contratuais: tempo de permanência, tipo de contrato, método de pagamento, cobrança eletrônica, valores mensais e totais.
Dados demográficos: gênero, faixa etária, presença de dependentes ou parceiros.
3. Metas do Projeto
Analisar detalhadamente cada variável.
Realizar análise exploratória dos dados.
Tratar valores ausentes de forma adequada.
Dividir os dados em treino (80%) e teste (20%).
Converter variáveis categóricas em numéricas.
Treinar e validar modelos, começando por árvore de decisão.
Exibir e interpretar a matriz de confusão.
4. Modelos e Avaliação
Modelos Utilizados
Decision Tree
Random Forest
XGBoost
Logistic Regression
Support Vector Classifier (SVC)
Critério de Avaliação
Neste projeto, o foco está em maximizar o recall, visando identificar o maior número possível de clientes propensos a evasão (mesmo que tenhamos mais falsos positivos).

Reamostragem
5. Conclusões
O modelo que apresentou o melhor desempenho foi o SVC, após otimização dos hiperparâmetros.
As métricas ROC-AUC e PR-AUC (essencial para classes desbalanceadas) indicam que o modelo aprendeu bem e atingiu o objetivo empresarial.
Como esperado, houve um número relevante de falsos positivos devido ao foco em recall.

