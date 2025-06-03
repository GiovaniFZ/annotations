## Tipos de autenticação

1. Básica (Basic Auth)
- Faz com que, em todas as requisições, o usuário e a senha sejam enviados no cabeçalho da requisição.
- Não é uma boa prática, pois a senha é enviada em texto plano, o que compromete a segurança (Não é muito legal mandar a senha e o email do usuário toda vez que eu mande a requisição).
- É usada principalmente para testes.

2. JWT (JSON Web Token)
- O usuário primeiro envia o email e a senha para o servidor
- O servidor verifica se o email e a senha estão corretos
- Se estiverem corretos, o servidor gera um token único (não modificável e stateless)
- Stateless: Não é armazenado em nenhuma estrutura de persistência de dados (BD)
- O token é enviado para o usuário, e ele será usado nas requests.
- Quando o backend vai criar o token, ele usa uma palavra chave (string). Quanto mais difícil for, mais seguro será.
- Essa palavra chave é usada para verificar se o token é válido ou não.
- O token é composto por 3 partes:
    - Header: É o tipo de algoritmo que será usado para gerar o token (algoritmo de criptografia)
    - Payload: É o conteúdo do token (dados do usuário)
    - Signature: É a assinatura do token, que é gerada a partir do header, payload e a palavra chave.
- Convenção: Usar sub para identificar o usuário no payload. Ao mudar o sub, o token será inválido, pois a assinatura mudará.