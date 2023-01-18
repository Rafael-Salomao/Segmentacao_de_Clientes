# Segmentacao_de_Clientes

<p align="center">
  <img width="600" height="300" src="imagem01.png">
</p>

## 1.0 Introdução

Neste projeto, vamos fazer um trabalho de segmentação de clientes. O intuito é poder fazer campanhas mais direcionadas a um determinado público que tem uma maior propensão ao consumo de um produto, tipo de oferta etc.

## 2.0 Qual problema foi resolvido

Uma loja de um shopping quer entender melhor o perfil de seus clientes. O estabelecimento conta com algumas informações da sua carteira de clientes.

No atual cenário, o dono do comercial não sabe dizer claramente quem são seus melhores clientes e qual tipo de produto oferecer a fim de resultar em aumento de vendas. Para isso, o ideal seria entender o perfil de seus clientes, para melhor atendê-los.

Por conta disso, o gerente responsável contratou um cientista de dados para responder as seguintes questões:

- Em quantos segmentos é possível separar os clientes?
- Separar os clientes em diferentes segmentos.
- Qual a idade média dos clientes dentro de cada cluster?
- Qual o salário médio dos clientes dentro de cada cluster?
- Quais insight podemos ter a cerca do perfil dos clientes dentro de cada cluster?
- Quem é o segmento de clientes alvo para aumentar o faturamento da loja?

## 3.0 Como foi resolvido

Para a resolução do problema, foi aplicado um modelo estatístico muito utilizado na segmentação de clientes, o K-Means.

O problema se trata de um aprendizado não-supervisionado. Ou seuja, o modelo encontra semelhanças entre os diferentes clientes e os separam em clusters, sendo o K-Means, um modelo simples e eficiênte para esta prática.

Separar em clusters, é a tarefa de agrupar um conjunto de objetos de forma que os individuos presentes no mesmo cluster sejam mais semelhantes entre si do que em os presentes em outros clusters.

Para este projeto, ao utilizar o modelo de segmentação K-Means, é esperado que ao final dele seja obtido o segmento em que cada um dos clientes se encaixa. Em complemento a isso, o número de clusters que melhor satisfaz a necessidade do negócio, será definido por meio da análise do score do modelo. Sendo que, esta análise, será feita a partir da visualização do Elbow Graph e Silhouette Analysis.

## 4.0 Estrutura do projeto.

A estrutura do projeto foi elaborada com base no framework CRISP-DM. Por conta disso, a resolução do problema, introduzido anteriormente, será apresentada por meio dos seguintes tópicos:

- Exploração dos dados
- Preparação dos dados
- Construção do modelo
- Avaliação dos resultados
- Deploy e conclusão

## 5.0 Tecnologias utilizadas

- Pandas
- Numpy
- Matplotlib
- Pyplot
- Seaborn
- Scipy
- Sklearn
- Pickle
- Yellowbrick

## 6.0 Resultados obtidos

A partir das análises do Elbow Graph e Silhouette Analysis foi identificado que o melhor numero de clusters para esta base de dados, é de 5 segmentos de clientes.

Com essa segmentação, foi possível observar dois pontos inicial:

- Os Clusters 3 e 4, representam os clientes com maior score, são compostos por clientes de classe média, na faixa de 25 a 32 anos.
- De acordo com os Clusters 0, 1 e 2; clientes com idade maior que 40 anos, tendem a ter um menor score, no shopping. Sendo que, os de média salarial de 55k, contam com a maior quantidade de clientes, podendo ser um nicho promissor para o shopping atuar e aumentar suas vendas.

Após isso, foi analisado o perfil médio dos clientes dentro de cada um dos clusters e foi possível tirar as conclusões abaixo, sobre cada segmento de cliente para esta loja:

- Cluster 0: composto majoritariamente por mulheres, média de idade 42 anos, salário médio 55k. Tem um score de 49 e representa cerca 40,5% da carteira de clientes. (Média populacional)

- Cluster 1: composto majoritariamente por homens, média de idade 41 anos, salário médio 88k. Tem um score de 17 e representa cerca 17,5% da carteira de clientes. (Maior salário e mais velhos - Poucas oportunidades)

- Cluster 2: composto majoritariamente por mulheres, média de idade 45 anos, salário médio 26k. Tem um score de 20 e representa cerca 11,5% da carteira de clientes. (Menor salário e mais velhos - Poucas oportunidades)

- Cluster 3: composto majoritariamente por mulheres, média de idade 25 anos, salário médio 55k. Tem um score de 79 e representa cerca 11,0% da carteira de clientes. (Clientes em potencial)

- Cluster 4: composto majoritariamente por mulheres, média de idade 32 anos, salário médio 86k. Tem um score de 82 e representa cerca 19,5% da carteira de clientes. (Clientes estratégicos)

## 8.0 Agradecimentos e referências

[1] Modelo STP: Descubra a melhor maneira de colocar suas estratégias de comunicação em prática. Camelo Digital, 2022. Disponível em: < https://camelo.digital/2021/03/01/modelo-stp/ >. Acesso em: 10, dezembro de 2022.
