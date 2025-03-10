# Formas de o front end enviar requisições

## Query parameters
- São parâmetros nomeados, por exemplo, no link http://localhost:3333/?userid=1, userid é um query parameter.
- Usadas em URLs Stateful, isto é, usados quando enviamos informações não sensíveis, para modificar a resposta do BE.
- Exemplos: Filtros, paginação, etc.
## Route parameters
- Usados para identificação de um recurso. Por exemplo, no link http://localhost:3333/1, o identificador 1 é usado.
- Não precisa ter um nome, pois o método HTTP já identifica o que queremos.
## Request Body
- Envio de informações de um formulário, podemos ter n informações possíveis
- Mais difíceis de serem interceptados.