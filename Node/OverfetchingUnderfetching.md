# Overfetching e underfetching
- **Overfetching**: Quando a gente retorna informações demais para o front-end em rotas que não precisamos daquelas informações.
Por exemplo, se em algum momento eu precisar buscar os dados da pergunta sem as repostas?
Lembrar que quanto mais bytes, mais tempo de resposta
- **Underfetching**: Não podemos fazer micro rotas (pedacinhos). Fazer muitas requisições para obter os dados em tela é ruim.
Solução: Chegar no meio termo.