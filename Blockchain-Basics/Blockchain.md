# *Blockchain*

## O que é _Blockchain_? ⛓️

Como o próprio nome diz, a _Blockchain_ é uma cadeia de blocos conectados entre si, que contêm dados armazenados dentro dele. Esses dados podem ser qualquer coisa que pode ser guardada computacionalmente, como, por exemplo, informações de transações, imagens, textos e tudo mais. 

>
### Considerações ❕
Sim, a Blockchain está muito atrelada ao funcionamento do _Bitcoin_, porém, vamos deixar claro a sua total individualidade com relação à moeda. Apesar do nome "_Blockchain_" ser geralmente interligado, ou até mesmo confundido, com criptomoedas como o Bitcoin, a tecnologia é utilizada em muitos outros campos do desenvolvimento, como o campo farmacêutico, logístico, transporte, etc. O bitcoin utiliza de forma muito eficiente todas as **características** da Blockchain. 💰

---

Antes de começarmos a entender como funciona uma Rede _Blockchain_, vamos passar pelas características gerais que tornam a _Blockchain_ uma tecnologia com grande potencial. Não se preocupe com alguns termos ainda não vistos, desvendaremos todos de acordo com desenrolar do resumo. 😉

## Características 	📑
1. Transparente: A rede _Blockchain_ permite que todos os usuários da rede possam avaliar as informações registradas nela, validando ou não as informações novas através do **Protocolo de Consenso**;
2. Imutável: Através do uso de **Funções _Hash_**, a rede _Blockchain_ é imune a mudanças de informações já registradas na rede;
3. Descentralizada: Uma rede _Blockchain_ não possui uma entidade maior que a administra, ao invés disso, ela é uma rede _Peer-to-Peer_, ou seja, de "pessoa para pessoa", direta entre os usuários, sem intermediários, onde todos da rede têm acesso a ela e decidem como ela progride;
4. Irreversível: Pela natureza Imutável da _Blockchain_, é impossível reverter algum bloco antes inserido na rede, isso permite uma alta gama de aplicações que necessitam dessa característica.

---

![Imagem da _Blockchain_](https://www.cache2net3.com//Repositorio/251/Publicacoes/25278/6f452d7e-f.png)

---

## Funcionamento 🛠️
Mas como realmente funciona uma _Blockchain_?

A _Blockchain_ só é possível graças a existência de **Funções _Hash_**. Uma Função _Hash_ é um algoritmo matemático para criptografia, na qual acontece uma transformação de um certo dado de entrada(*Input*) em um conjunto alfanumérico com um comprimento fixo de caracteres(Soma _Hash_).

![Imagem do funcionamento de uma Função Hash](https://www.freecodecamp.org/portuguese/news/content/images/2022/09/Hash_function_long.png)

## Propriedades de uma Função _Hash_ ⚙️

1. Fácil de computar - "Fácil" no quesito computacional, ou seja, é muito fácil para o computador fazer esse cálculo;
2. Livre de colisão - É praticamente* impossível dois _inputs_ terem o mesmo resultado na Soma _Hash_;
3. Unidirecional - Isso quer dizer que, dado um certo número resultado de uma Função _Hash_, é praticamente* impossível descobrir qual foi o _Input_ que resultou nela;
4. "_Puzzle Friendly_" - Dado um input, qualquer mínima mudança nele resulta em Somas _Hash_ **completamente** diferentes, não importa se a mudança for um caractere a mais ou a menos. Inclusive, a exemplo, mesmo o _input_ sendo de dois caracteres, a Soma _Hash_ continua sendo de tamanho fixo.

> " * " O "praticamente" nos tópicos 2 e 3 pois teoricamente, se fossem dados infinitos de inputs, haveria dois com o mesmo resultado _Hash_, mas na prática, isso é muito, muito improvável.

## Mas como funciona o cálculo da Soma _Hash_? 🔢

Como dito anteriormente, os blocos na _Blockchain_ armazenam dados, porém, além desses dados, os blocos armazenam o código _Hash_ do bloco antecessor a ele, chamamos isso de _Hash Pointer_(Ponteiro _Hash_), pois ele aponta para o bloco anterior na rede. 
Então, diante disso, os _Hash_ são criados a partir do _Hash_ do bloco anterior em conjunto com os dados armazenados no bloco. 
### Tentativa de fraude 👨‍💻
Pela natureza de como se estrutura os blocos, a _Blockchain_ é **imutável**, pois uma vez que qualquer dado seja adulterado, o _Hash_ daquele bloco muda completamente graças a capacidade _Puzzle Friendly_, sendo assim, toda a rede receberá e perceberá a mudança do _Hash_, causando então o alerta de alteração.

---
## Demonstração 🧐
Aqui está um site que demonstra visualmente como funciona uma blockchain, onde você pode criar e interagir com o blocos, observando como funciona as características de uma rede _Blockchain_, anteriormente mostradas aqui. [Clique aqui](https://blockchaindemo.io) para ir até a demo. 

---

## Protocolo de Consenso 🧑‍🤝‍🧑

Foi dito anteriormente que a _Blockchain_ toma decisões a partir de um consenso, isso se dá ao fato de que a rede é distribuída a todos. Cada computador conectado a rede _Blockchain_ possui uma cópia de toda a rede, possuindo os registros de tudo que aconteceu nela desde o **_Gênesis Block_** até o último bloco criado.

> _Gênesis Block_ é o bloco inicial da cadeia _Blockchain_. 🔝

Diante disso, cada usuário, ou nó da rede(computador conectado) pode analisar as informações contidas na cadeia, decidindo, por exemplo, aprovar ou não a criação de um bloco específico. Se o consenso dos nós ser atingido, o bloco é incluído na cadeia, sendo trabalhado a partir dele, caso contrário, a ramificação é ignorada e todos seguem, por onde for julgado, um bloco verídico. 

---


## Mas como a _Blockchain_ pode ser implementada? 🤔
Para isso, podemos analisar como o próprio Bitcoin funciona, pois lá veremos como uma _Blockchain_ pode ser usada para criar mecanismos interessantes na área de desenvolvimento, utilizando de todos os conceitos que foi explicado aqui. Te vejo no resumo sobre [Bitcoin](/Blockchain-Basics/Bitcoin.md). 😉

[Voltar ⬅️](Bitcoin.md)

[Voltar ao inicio 🔙](../README.md) 