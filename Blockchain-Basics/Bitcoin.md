# _Bitcoin_ 

## O que é _Bitcoin_? 💰
_Bitcoin_ é uma moeda virtual, ou criptomoeda, como ficou mais conhecida, cuja característica é ser uma moeda **descentralizada** não dependente de uma instituição intermediária, como o dinheiro tradicional funciona com os bancos. Com essa descentralização, o _Bitcoin_ tem o objetivo de trazer uma **transparência** para todos que o utilizam.

Com essas premissas, remete a algo? Sim, a [_Blockchain_](/Blockchain-Basics/Blockchain.md). ⛓️

> Vamos esclarecer como funciona o _Bitcoin_ e qual a sua relação com uma rede _Blockchain_, por isso é interessante você saber como funciona uma _Blockchain_, que há um resumo [aqui](/Blockchain-Basics/Blockchain.md). 👍

---
Antes de começar a entender o funcionamento técnico da moeda, podemos analisar como ela surgiu e, principalmente, como suas **propostas** se interligam com as **características** da _Blockchain_.

## Como surgiu o _Bitcoin_? 📜
O _Bitcoin_ surgiu diante da crise dos bancos de 2008 nos Estados Unidos, quando os bancos não cumpriram com suas _promessas_* e abalaram as confianças de seus clientes, causando uma grande crise financeira no país. Diante disso, muitos sentiram a necessidade de alguma forma de tornar seu dinheiro algo mais controlável e independente de órgãos maiores.

> \* A dita "promessa" é como funciona o sistema financeiro tradicional, que, quando é colocado um dinheiro na conta em um banco, é como se o banco fizesse uma promessa que, quando necessitado pelo cliente, ele entregará a quantia desejada. Porém o dinheiro do cliente não é armazenado totalmente, é reservado uma pequena parte e o restante é investido aos interesses do banco ou "emprestado" a outros clientes, essa é a chamada "Reserva Fracionária".

Diante de toda essa situação, em 2009 surgiu na internet o pseudônimo chamado Satoshi Nakamoto, com a ideia de uma moeda totalmente descentralizada e transparente, o _Bitcoin_. A quesito de curiosidade, nem ao menos sabemos se Satoshi Nakamoto é uma pessoa ou um grupo de pessoas. De qualquer forma, a criação da moeda pôde nos proporcionar uma rede _Blockchain_ que funciona de forma interessante para analisarmos, então, vamos à parte técnica.

---
![Imagem de como funciona o _bitcoin_](https://arxiv.org/html/2403.14854v1/extracted/5487265/transaction.png)

## Como funciona o _Bitcoin_?🛠️
A partir da origem do _Bitcoin_, podemos assimilar com o funcionamento da _Blockchain_. As ideias do _Bitcoin_ puderam ser intercaladas e implementadas com as características da _Blockchain_. A _Blockchain_ do _Bitcoin_ é um registro público e imutável de todas as transações já realizadas desde a criação do _Bitcoin_, armazenados em blocos montados como na imagem abaixo:
![Imagem de como é um bloco na rede Blockchain do Bitcoin](https://miro.medium.com/v2/resize:fit:700/0*Scr0R4kBixv8lEFt.png)


Vamos então analisar como o _Bitcoin_ entrega autenticidade e transparência partir das características presentes na _Blockchain_.

# Propriedades do _Bitcoin_ ⚙️
## Assinaturas Digitais 📝
Para realizar transações na rede _Bitcoin_, é necessário uma assinatura digital que possui as mesmas propriedades de uma assinatura tradicional, são elas:

1. Só você pode assinar;
2. Qualquer pessoa pode verificar sua assinatura;
3. A assinatura deve ser atrelada a uma única transação, ou seja, ninguém pode copiar sua assinatura e colar em outro lugar.

Essas assinaturas só podem ser criadas e autenticadas a partir de um mecanismo de segurança chamado **Criptografia de Chave Pública**.
## Chaves 🔑
### Chave Pública 📭
- É a sua **identidade** na rede _Bitcoin_, deve ser, como o próprio nome diz, público para servir como um endereço onde todas as transações devem "apontar" para ela. 
- Os usuários não possuem uma conta como nos bancos tradicionais, ao invés disso, a rede calcula quantos _Bitcoins_ foram transferidos para as chaves públicas e quantos ainda não foram gastos.
### Chave Privada 🔐
- Essa é a chave necessária para realizar as transações, com ela, a partir de uma função matemática complexa, o usuário cria suas assinaturas digitais para serem enviados na transação. A **única** forma de criar uma transação é com a chave privada.


## Verificação de transações 💼🧐
Através também de uma função matemática, é possível verificar a veracidade das transações a partir da assinatura na transação e a chave pública de quem realizou a mesma. Assim, todos na rede podem analisar as transações de todos.

Cada usuário pode ter **diversas** chaves públicas, cada uma atrelada a uma chave privada diferente. Portanto, enquanto o usuário estiver com a chave privada, poderá realizar as transações das suas respectivas chaves públicas.

![Imagem que demonstra o processo de assinatura e verificação de transações](https://www.mycryptopedia.com/wp-content/uploads/2017/09/Digital-Signatures.jpeg)

---

## Risco de Fraudes 👨‍💻
O _Bitcoin_ utiliza da **Imutabilidade** da _Blockchain_ para que transações não sejam falsificadas ao estarem na rede. Porém, como foi dito, transações dependem das chaves privadas, portanto, se o usuário tiver sua chave privada vazada ou roubada, todos os seus _Bitcoins_ estarão em risco, visto que a rede não entende a veracidade de quem está fazendo a transação, ela apenas verifica se a chave pública e privada estão atreladas e realiza a transação. Lembrando que, uma vez realizada qualquer transação, **não há como retornar**.
Por isso, ataques _Hackers_ são direcionados a descobrir as chaves privadas de usuários, e não a rede em si, visto que é impossível alterar qualquer dado na _Blockchain_.

---

## Rede _Bitcoin_ 👥

Foi dito anteriormente que todos na rede _Bitcoin_ podem verificar as transações de todos os outros usuários conectados a rede. Os nós na rede podem utilizar de duas classificações de rede em seus computadores, são eles os _Full Nodes_ e os _Lite Nodes_.

- _Full Nodes_:
  - Têm toda a rede _Blockchain_ em seus computadores;
  - Validam todas as transações;
  - Mantêm a consistência da _Blockchain_
- _Lite Nodes_:
  - Não armazenam toda a _Blockchain_, apenas o necessário para seu funcionamento;
    - Esse tipo de rede funciona melhor em dispositivos menos eficientes como, por exemplo, em celulares.
  - Se necessitarem de alguma informação externa, buscam nos _Full Nodes_;
    
![Rede bitcoin](https://icoda.io/wp-content/uploads/2023/08/protocol8.png)

---

## Protocolo _Gossip_ 🖥️ 🗨️ 🖥️
O Protocolo _Gossip_, ou Protocolo de Fofoca, é um protocolo de comunicação que permite com que os dispositivos digitais possam propagar uma informação na rede _Peer-to-Peer_* de forma rápida e confiável entre si. 

No _Bitcoin_, o Protocolo de Fofoca funciona logo após ser registrado uma nova transação na rede. Um dos nós, então, informa a outro que houve uma nova transação, passando todas as informações como, quais _Bitcoins_ foram usados, a chave pública destino e a sua própria chave, assim, o nó que recebe isso espalha para todos os outros nós que aquela transação aconteceu.

> \* _Peer-to-Peer_ é mais uma caracteristica do _Bitcoin_ que pôde ser instaurada a partir da Blockchain, alcançando assim, o objetivo de não haver intermediários entre as transações.

![Imagem protocolo de fofoca](https://bpcdn.co/images/2022/02/17194943/bitcoin-network-message-propogate.png)

---

## Mineradores ⛏️

Os Mineradores da rede _Bitcoin_ ficaram muito famosos no boom do _Bitcoin_, mas afinal, **o que fazem os Mineradores?**

- Os Mineradores da rede _Bitcoin_ validam as transações recebidas e criam novos blocos para serem inseridos na cadeia da Blockchain;
- Concorrem para decidirem quem vai ter o direito de adicionar um novo bloco à rede;
- Verificam blocos obtidos por outros mineradores e colocam na _Blockchain_, se validado;
- Sempre estendem o ramo mais longo da _Blockchain_.

## _Proof of Work_ 👷‍♀️

Para adicionarem o bloco a rede, os mineradores, além de validar todas as transações para inserirem ao bloco, devem encontrar uma saída _Hash_ com um determinado número de zeros ao início. Esse Hash só é encontrado a partir de um número inteiro específico, chamado de **_Nounce_**, que, deve ser combinado com os dados do bloco(transações) na função _Hash_. O _Nounce_ certo é aleatório, logo, os mineradores precisam ficar chutando números inteiros até achar o _Nounce_ que os levem até a saída necessária.

![Imagem que mostra a Dificuldade](https://paymentandbanking.com/wp-content/uploads/2020/03/Screenshot-2020-03-23-at-21.39.38-1140x556.png)

> A quantidade de zeros ao início do código hash determina a dificuldade para conseguir validar o bloco, quanto mais zeros, mais díficil é de achar o _Nounce_ correto.
> > Na rede do Blockchain do _Bitcoin_, deve haver um novo bloco a cada 10 min, e dependendo da quantidade de mineradores, a dificuldade diminui ou aumenta, logo, a rede nunca será afetada pela perda de mineradores.

Ao achar um Bloco válido, o minerador tem o direito de fazer uma **_Coinbase Transaction_**, que permite criar uma quantidade de _Bitcoins_ e endereçá-los para alguém, geralmente a ele mesmo, como recompensa. Essa é a chamada _Proof-of-Work_(Prova de Trabalho) dos mineradores.

## Tempo no _Bitcoin_ ⏳

A cada 4 anos, a quantidade de _Bitcoin_ criada nas _Coinbase Transactions_ cai pela **metade**. Sendo assim, daqui a alguns anos, a única forma dos Mineradores ganharem _Bitcoin_ será a partir da tarifa* aplicada nas transações.

> \* Tarifa aplicada quando ocorre uma transação - sempre é enviado um pouco a mais de _Bitcoin_ que o necessário nas transações, como forma de tarifa aos Mineradores que validam os blocos.

---

## Protocolo de Consenso 💬
Ainda quando um bloco é validado por um minerador, os outros mineradores analisam aquele bloco e, se julgarem como verídicos, começam a minerar a partir daquele bloco, caso contrário, continuam minerando do bloco antigo e essa ramificação é ignorada. Por isso é dito que os Mineradores sempre entendem o ramo mais longo da blockchain.

---

## Finalização 🤔
Então é assim que funciona o Bitcoin, é um sistema que pode explicar perfeitamente como funciona uma Rede Blockchain e é um exemplo claro do potencial da tecnologia!

Enfim, é isso, há muitos outros detalhes como a organização dos Mineradores, tentativas de Gasto Duplo e como o Protocolo de Consenso consegue lidar com elas, mas são detalhes extras.

[Voltar ⬅️](../Blockchain-Basics/)

[Voltar ao início 🔙](../README.md) 