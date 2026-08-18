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

# Itens que compõem o funcionamento da blockchain:
1. Transação (Registro digital de transferência de moedas). É formado por: **id, entrada, saída, quantidade e marcação de tempo**.
2. Bloco (Conjunto de transações)
3. Hash (Função que tem o objetivo de compilar dados de qualquer tamanho para um fixo)
4. Livro razão (ledger): Registro das transações

# Itens - transação
1. ID: Identificador único formado por função hash.
2. Entrada: Endereço de quem está enviando dados
3. Saída: Endereço de quem está recebendo
4. Quantidade: Valor que será transferido
5. Marcação de tempo: Registro de data/hora.

# Chave pública e privada
- São usadas na assinatura das transações a fim de manter o anonimato. A **criptografia de chave pública** faz uso de um par de chaves matematicamente conectadas. A **chave pública** é gerada a partir da **chave privada**. O inverso não pode acontecer.
- Para produzir um endereço Bitcoin, portanto, utilizamos a chave privada do usuário, e a partir dela, a pública. Ao submeter a pública em um algoritmo SHA-256, obtemos nosso endereço, que será submetido ao RIPEMD-160, gerando o endereço Bitcoin.

# Bloco Gênesis
- É o bloco inicial, não possui registros de outros blocos então o hash do bloco anterior nesse caso é marcado como 0.
- Merkle Root Hash: Árvore de transações
- Curiosidade: O timestamp do bloco é marcado como um número no padrão Unix (Ex: 1533750000).

# Funções Hash
- Não é possível saber os dados iniciais a partir de um hash.
- SHA-256 é o mais utilizado

# Livro razão - ledger
- Cada nó possui uma cópia do livro razão, sendo assim, qualquer modificação do livro seria reconhecida pelos nós.

# Mineradores
- São responsáveis por resolver um desafio (prova de trabalho) para cada transação, que consiste em incrementar o valor NONCE do bloco até que a hash do bloco apresente um determinado número de zeros iniciais. O primeiro que soluciona compartilha para os demais nós para validação.
- Mineração de dados exige alto poder computacional pois envolvem cálculos complexos. Dessa forma, o trabalho pode ser dividido.
- Exemplo: Supondo que o desafio seja pegar uma palavra, e devemos fazer com que o target value seja 2 (ou seja, deve ter dois zeros iniciais). Para isso, usamos o nonce, que será adicionado na palavra. O computador precisa executar x vezes até que o hash comece com 2 zeros.
- Ou seja, o **nonce** é o número de tentativas para se chegar em um hash válido.
- Somente após 51% de validação, a transação é validada e o bloco é incluído na cadeia.
- Ver: http://www.blockchain-basics.com/HashPuzzle.html
