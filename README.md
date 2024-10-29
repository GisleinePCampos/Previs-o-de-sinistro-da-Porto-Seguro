# Previsão-de-sinistro-da-Porto-Seguro
![image](https://github.com/user-attachments/assets/db7e4e91-18a1-4376-abd9-ecd10939d01e)

Contratar um seguro de carro é uma ótima opção para se proteger e evitar dores de cabeça em caso de danos ao veículo e ao motorista. O seguro de carro é um tipo de contrato que firma a obrigação da seguradora em cobrir o motorista e o veículo contra possíveis danos ou responsabilidades que possam surgir em caso de acidente de trânsito. 

O funcionamento de um seguro de carro é baseado em um contrato de seguro no qual uma seguradora se compromete a indenizar o segurado por danos ao seu veículo ou por responsabilidade por danos causados a terceiros em troca do pagamento de um prêmio (valor) pelo seguro. Para adquirir um seguro de carro, o interessado deve procurar uma seguradora e fornecer informações sobre o veículo e o condutor. A seguradora usará essas informações para avaliar o risco de acidente e determinar o valor do prêmio.

A Porto Seguro, uma das maiores seguradoras de automóveis e residências do Brasil, concorda plenamente. Imprecisões nas previsões de sinistros de seguradoras elevam o custo para bons motoristas e diminuem para os ruins. Nesta competição, o desafio é construir um modelo que preveja a probabilidade de um motorista realizar um sinistro de seguro auto no próximo ano. Embora a Porto Seguro use aprendizado de máquina há 20 anos, eles buscam novos métodos através da comunidade de aprendizado de máquina do Kaggle. Uma previsão mais precisa permitirá ajustar melhor seus preços, tornando o seguro automotivo mais acessível a mais motoristas.

## Avaliação do Modelo (Sugerido pela Porto Seguro)
Métrica de Pontuação: As submissões são avaliadas usando o Coeficiente Gini Normalizado.

O Coeficiente Gini Normalizado ajusta a pontuação pelo máximo teórico, de modo que a pontuação máxima é 1.

## Entendimento do problema de negócio
Construir um modelo que preveja a probabilidade de um motorista fazer um sinistro de seguro auto no próximo ano. 

Sinistro é o nome dado quando há alguma ocorrência danosa com seu automóvel, configurada como perda total ou não, e o seguro é acionado. Ou seja, um sinistro é a classificação que um veículo ganha quando há uma colisão, furto ou um prejuízo dentro de alguma das formas previstas na apólice do seguro.

Após a ocorrência de um sinistro, o segurado deve entrar em contato com a seguradora para informar o ocorrido e iniciar o processo de avaliação e eventual indenização, conforme estabelecido na apólice de seguro.

## Entendimento dos dados
Para este projeto utilizaremos os dados disponibilizados pela seguradora Porto Seguro no ambiente Kaggle:

https://www.kaggle.com/competitions/porto-seguro-safe-driver-prediction/data

Nos dados de treinamento e teste:

variáveis que pertencem a agrupamentos semelhantes são marcadas como tal nos nomes das variáveis (por exemplo, ind, reg, car, calc).
Os nomes das variáveis incluem o sufixo "bin" para indicar variáveis binárias e "cat" para indicar variáveis categóricas. Variáveis sem essas designações são contínuas ou ordinais.
Valores de -1 indicam nulo.
A coluna "target" indica se uma reclamação (sinistro) foi feita ou não para aquele titular da apólice.

O arquivo train.csv contém os dados de treino, onde cada linha corresponde a um titular de apólice, e a coluna "target" indica que uma reclamação foi feita. O arquivo test.csv contém os dados de teste.
