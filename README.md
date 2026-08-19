# 🏋️ Fitness Gym Churn Analysis

## 📋 Descrição
Análise de dados para a rede de academias Model Fitness com o objetivo de identificar clientes com maior risco de churn e propor estratégias de retenção.

O projeto utiliza dados de comportamento, frequência, tipo de contrato e características dos clientes para entender os principais fatores relacionados ao cancelamento.

## 🎯 Objetivo
Criar uma estratégia de interação com os clientes baseada em dados, identificando perfis com maior probabilidade de cancelamento e oportunidades para aumentar o engajamento e a retenção.

## 📊 Dados
- `gym_churn_us.csv` - Dados de clientes da academia
	- Informações demográficas e de localização
	- Tipo e duração do contrato
	- Frequência de visitas e participação em aulas coletivas
	- Gastos adicionais e tempo de relacionamento
	- Indicador de churn

## 🚀 Como Executar
```bash
jupyter notebook analysis.ipynb
```

As principais bibliotecas utilizadas no projeto são `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy` e `scikit-learn`.

## 🔧 Etapas de Processamento
- Análise exploratória e descrição dos dados
- Verificação e tratamento da estrutura dos dados
- Análise da relação entre características dos clientes e churn
- Comparação de modelos de classificação
- Avaliação dos modelos usando acurácia, precisão e recall
- Padronização das variáveis para agrupamento
- Segmentação dos clientes com algoritmo K-Means
- Análise das métricas médias por cluster

## 🤖 Modelo de Classificação
Foram comparados modelos de classificação para prever o churn dos clientes. A `LogisticRegression` apresentou o melhor recall e foi selecionada como modelo mais adequado para identificar clientes em risco de cancelamento.

## 👥 Segmentação de Clientes
Os clientes foram divididos em cinco grupos com características distintas:
- **Risco Crítico**: contrato curto, baixa frequência e menor tempo de relacionamento
- **Altamente Engajados**: maior frequência e maior tempo de relacionamento
- **Alto Risco**: contrato curto e frequência baixa ou moderada
- **Fidelizados por Contrato**: contrato longo, mesmo sem o maior nível de engajamento
- **Risco Moderado**: contrato de duração média e métricas intermediárias

## 📈 Análises Realizadas
- Identificação dos fatores associados ao churn
- Comparação do comportamento entre clientes que cancelaram e clientes retidos
- Avaliação da influência da duração do contrato na retenção
- Análise da frequência de visitas e participação em aulas coletivas
- Identificação dos clusters com maior taxa de churn
- Visualização das métricas médias de cada grupo

## 💡 Conclusões
- O cluster de maior risco apresenta baixa frequência e menor tempo de relacionamento com a academia.
- Clientes com contratos mais curtos tendem a cancelar com maior frequência.
- A participação em aulas coletivas pode contribuir para a criação de hábitos e o aumento do engajamento.
- O acompanhamento dos clientes nos primeiros meses pode ajudar a reduzir o churn.
- Descontos e benefícios para contratos mais longos podem incentivar a retenção.
- Estratégias de gamificação e comunicação mais próxima podem aumentar o envolvimento dos clientes.

## 🛠️ Tecnologias
- **Python** 3.8+
- **pandas**, **numpy** - Manipulação e análise de dados
- **matplotlib**, **seaborn** - Visualização de dados
- **scipy** - Análise estatística
- **scikit-learn** - Modelos de classificação e clustering

