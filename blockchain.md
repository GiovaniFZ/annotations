# Blockchains
- São utilizadas em transações P2P. Envolve vários mecanismos, como a criptografia e o minerador também recebe recompensas.
- Impacta na redução de custos, rastreabilidade, transparência e segurança, eliminando desperdícios e corrupção.
- A intermediação é feita por mineradores. Supondo por exemplo que compramos um apartamento pela internet sem a intermediação de um banco. Provavelmente sem a blockchain, isso não seria viável, porém com ela, é possível que outras usuários (mineradores) consigam validar as informações, tanto em relação ao vendedor quanto em relação a quem está comprando (exemplo: se possui saldo disponível).

# Criptomoedas
- Exemplo: Bitcoin: envolve criptografia como elemento de segurança
- Possuem o anonimato como característica principal entre as partes que negociam
- A troca fincanceira acontece sem intermédios
- A tecnologia que está por trás das transações de criptomoedas como o bitcoin é a Blockchain.

# Sistemas de rede
- Centralizado: Um servidor armazena informações e controla as tarefas e os serviços realizados por usuários conectados a ele. Nessa rede, todas as partes ou computadores dependem de um ponto (computador central) para distribuir a informação para os demais computadores.
- Distribuído: Todos os usuários estão interconectados e a comunicação ocorre diretamente entre as partes, por isso, a expressão ponto a ponto (P2P). Não existe um servidor central que controla e registra as transações. Em uma transação, a informação na rede deve ser confirmada por pelo menos 51% dos nós, isso garante também que a data das transações (linha do tempo) não seja modificada.

# Registro da transação
- Ledger: Livro razão onde são feitos os registros das transações.
- Cada transação envolve um ou mais endereços, e o registro de um evento deve ser digitalmente assinado para garantir autenticidade da transação.
- Cada transação, ou conjunto de transações, forma um bloco que é adicionado a outros blocos. Esses blocos formam uma cadeia.

# Fluxo da informação
1. Ocorre a solicitação feita por você
2. A solicitação é transmitida para os nós mineradores
3. Os nós mineram os dados para verificar se estão corretos, para assim validar a negociação. Eles competem para decodificá-las e disponibilizar na rede primeiro, dessa forma eles precisam de super computadores com alto processamento de cálculos. O trabalho de mineração é remunerado com criptomoedas.
4. O primeiro computador que resolver o cálculo disponibiliza o bloco de informações com a solução na rede. Os outros nós verificarão se a solução é válida.
5. Após validado, o novo bloco é adicionado a cadeia de blocos de modo permanente e inalterável. Eles possuem 2 códigos hashes para segurança.
**Curiosidade:** Alguns computadores possuem o histórico completo de transações da blockchain. Eles são chamados de **fullNodes**.
