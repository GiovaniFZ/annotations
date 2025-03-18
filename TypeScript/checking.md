## Runtime Type Checking
A validação de tipo de dados ocorre em tempo de execução. Usado no JavaScript.
Exemplo:
```
function calculateAge(user){
    return new Date().getFullYear() - user.birthDate
}
```
## Static Type Checking
A validação de tipo de dados ocorre enquanto a aplicação está sendo desenvolvida. Usado no TypéScript.
- No TS, Podemos usar interface ou Type para informar qual é o tipo de formato que se espera obter:
```
interface User {
    birthDate: number
}
```

## Resumo
- O TS permite evitar vários problemas futuramente, a partir da tipagem dos dados.