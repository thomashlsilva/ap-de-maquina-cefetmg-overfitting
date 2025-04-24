# Atividade: Implementação de Decision Tree Classifier e Overfitting

## Descrição

Esta atividade implementa o modelo de **Decision Tree Classifier**, um algoritmo fundamental de aprendizado supervisionado. O foco principal da atividade é:

- Implementação do modelo para classificação.
- Análise e prevenção de **overfitting** ajustando o parâmetro `min_samples_split`.
- Avaliação do modelo utilizando **Acurácia** e posteriormente **classification_report**.
- Testes automatizados para validação da implementação.

---

## Conceitos Implementados

### 1. `cria_modelo()`
Esta função implementa o modelo de árvore de decisão para classificação. A árvore é construída a partir de divisões nos dados, de acordo com um critério de ganho de informação. O modelo é ajustado utilizando o parâmetro `min_samples_split` para controlar a divisão das amostras em cada nó da árvore.

- O parâmetro `min_samples_split` é ajustado para otimizar o modelo e prevenir o **overfitting**.
- O modelo é treinado utilizando o conjunto de treinamento e avaliado nos conjuntos de validação e teste.

### 2. `divide_treino_teste()`
Função que divide os dados em dois conjuntos, sendo a proporção um valor de 0 a 1, sendo que 1 representa 100%:

- **Treinamento**: Conjunto utilizado para treinar o modelo.
- **Teste**: Conjunto final utilizado para avaliar o desempenho do modelo.

### 3. `faz_classificacao()`
Função responsável por treinar e avaliar o modelo **Decision Tree Classifier**, utilizando os conjuntos de treino e teste.

### 4. `plot_performance_min_samples`
Função para plotar a variação da acurácia com `min_samples_split` do modelo de árvore de decisão.

---

## Testes

O arquivo `overfitting_test.py` valida os seguintes componentes:

- A divisão correta dos dados em treino e teste.
- A implementação do modelo **Decision Tree Classifier**.
- O cálculo de **Acurácia**.

Todos os testes passam com sucesso, validando a implementação do modelo e a prevenção de overfitting.

---

## Instruções de Execução

### Instalação de Dependências

Certifique-se de ter o Python e os pacotes necessários instalados:

```bash
apt-get install python3 jupyter python3-pip
pip install -r requirements.txt
```

Atenção: Evite usar sudo com o pip.

### Executando o Jupyter Notebook

```bash
jupyter notebook
```
Abra o notebook fornecido e execute as células conforme as instruções no arquivo.

---

## Créditos

Atividade desenvolvida para a disciplina de Machine Learning do CEFET-MG, Campus Nova Gameleira.

Material baseado nas aulas do professor Daniel Hasan Dalip.