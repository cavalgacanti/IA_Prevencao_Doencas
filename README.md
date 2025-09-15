# IA_Prevencao_Doencas

# 1- O que significa classificação supervisionada?
Classificação supervisionada é um tipo de aprendizado de máquina em que o modelo é treinado com dados que já têm a resposta correta
a classificação supervisionada é usada para prever se um tumor é benigno ou maligno, aprendendo com exemplos já classificados. Os modelos utilizam essas informações rotuladas para generalizar e classificar novos casos.

# 2- Qual é a importância de dividir o dataset em conjunto de treino e teste?
Dividir o dataset em treino e teste é importante para avaliar se o modelo realmente aprendeu os padrões dos dados ou se apenas “decorou” os exemplos.
Conjunto de treino: usado para ensinar o modelo, ajustando os parâmetros a partir dos exemplos.
Conjunto de teste: usado para medir o desempenho em dados novos, simulando situações do mundo real.

# 3- Qual a diferença entre Decision Tree e KNN em termos de funcionamento?
A Decision Tree cria regras de decisão durante o treino, formando uma árvore que classifica os dados rapidamente e é fácil de interpretar, mas pode sobreajustar. 
O KNN não treina um modelo, apenas armazena os dados de treino e classifica novos exemplos com base nos vizinhos mais próximos, 
sendo sensível à escala das features e mais lento em grandes conjuntos de dados.

# DATASET
O dataset utilizado foi o Pima Indians Diabetes Database, disponível no Kaggle. 
Ele contém informações médicas de 768 pacientes mulheres com mais de 21 anos da tribo indígena Pima, localizada no Arizona (EUA).

# Resultado

Decision Tree
Acurácia: 0.7272727272727273
Matriz de Confusão:
 [[85 15]
 [27 27]]

 KNN
Acurácia: 0.7012987012987013
Matriz de Confusão:
 [[80 20]
 [26 28]]

 Logistic Regression
Acurácia: 0.7142857142857143
Matriz de Confusão:
 [[82 18]
 [26 28]]

# Qual modelo apresentou melhor desempenho no dataset escolhido?
O modelo com melhor desempenho foi a Regressão Logística, apresentando maior acurácia em relação aos demais.

# O resultado faz sentido?
Sim. O dataset é formado por variáveis numéricas contínuas (como glicose, pressão e IMC), o que favorece a Regressão Logística, 
pois ela lida bem com relações lineares entre atributos e a variável alvo.

# O que poderia ser feito para melhorar os modelos?
Para melhorar os modelos, é possível tratar valores inválidos ou ausentes, normalizar os dados, balancear as classes, ajustar hiperparâmetros
Além disso, criar novas features a partir dos dados existentes pode aumentar a capacidade preditiva.
