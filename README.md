# Classificacao-de-Rocha-ou-Metal-via-Sonar-Classification--Rock-or-Metal--via-Sonar

Imagine que você recebeu dados de coleta de um sonar posicionado em algum ponto do oceano e sua tarefa é identificar qual tipo de objeto o sonar conseguiu captar com base nos sinais coletados.

O presente estudo busca trabalhar com classificação através de sinais deste sonar, de modo que temos as opções do sinal indicar uma rocha ou um cilindro de metal. Temos, para tanto, 60 parâmetros que são indicativos de qual tipo de objeto estamos trabalhando. Queremos, assim, responder algumas questões:

1. Como se dá a distribuição de cada um destes parâmetros;

2. Existe(m) algum(ns) parâmetros com valores muito discrepantes dos demais?

3. Qual a correlação entre os parâmetros? Podemos ignorar algum ou alguns de modo que a classificação não sofra perdas de acurácia?

E, por fim:

4. Dentre alguns métodos de classificação que iremos trabalhar (Support Vector Machine, Regressão Logística, Random Forest e Gradient Boosting), qual aquele que retorna melhor acurácia na classificação (rocha ou metal)?



![3-Figure2-1](https://user-images.githubusercontent.com/72801602/115872965-c965e280-a418-11eb-9fa6-d8e6f2e30eb0.png)



Endereço da imagem: https://d3i71xaburhd42.cloudfront.net/7bdaefdd9954b75fdf305135b27105214c8eac66/3-Figure2-1.png

# Fonte:

O conjunto de dados foi contribuído para a coleta de benchmark por Terry Sejnowski, agora no Salk Institute e na Universidade da Califórnia em San Diego. O conjunto de dados foi desenvolvido em colaboração com R. Paul Gorman, do Allied-Signal Aerospace Technology Center.

O arquivo "sonar.mines" contém 111 padrões obtidos através da projeção de sinais de sonar de um cilindro de metal em vários ângulos e sob várias condições. O arquivo "sonar.rocks" contém 97 padrões obtidos de rochas em condições semelhantes (total de 208 amostras entre metais e rochas). O sinal de sonar transmitido é um sinal chirp (varredura em frequência em regime transiente) modulado em frequência, aumentando em frequência. O conjunto de dados contém sinais obtidos de uma variedade de ângulos de aspecto diferentes, abrangendo 90 graus para o cilindro e 180 graus para a rocha. Ambos os alvos (rocha e cilindro de metal) tinham aproximadamente 5 pés (ft) de comprimento e os retornos foram coletados em um intervalo de 10 metros.

Cada padrão é um conjunto de 60 números no intervalo de 0.0 a 1.0. Cada número representa a energia dentro de uma determinada banda de frequência, integrada ao longo de um determinado período de tempo. A abertura de integração para frequências mais altas ocorre mais tarde, uma vez que essas frequências são transmitidas mais tarde durante o chirp.

O rótulo associado a cada registro contém a letra "R" se o objeto for uma rocha e "M" se for uma mina (cilindro de metal). Os números nas etiquetas estão em ordem crescente de ângulo de aspecto, mas não codificam o ângulo diretamente.

Links das fontes usadas:

Dataset utilizado:
https://sci2s.ugr.es/keel/dataset.php?cod=85

Descrição detalhada e referências:
http://archive.ics.uci.edu/ml/datasets/Connectionist+Bench+%28Sonar%2C+Mines+vs.+Rocks%29

Artigo que usa este dataset:

R.Paul Gorman, Terrence J. Sejnowski, **Analysis of hidden units in a layered network trained to classify sonar targets**, Neural Networks, Volume 1, Issue 1,
1988, Pages 75-89, ISSN 0893-6080,
https://doi.org/10.1016/0893-6080(88)90023-8.
(https://www.sciencedirect.com/science/article/pii/0893608088900238)
