# Debounce
- O que é?
Vamos supor que exista um campo de input, por exemplo de pesquisa e o usuário digita um valor.
Cada vez que esse valor mudar, será feita uma nova chamada a API.
Porém queremos evitar chamadas desnecessárias para a API para questões de otimização.
Ao fazer o debounce da função que faz o set do valor do input, a ideia é aguardar um tempo para que ele guarde o valor do input e aí sim envie os dados para a API.

# Exemplo de implementação - TypeScript
```ts
// eslint-disable-next-line
export function debounce<T extends (...args: any[]) => any>(
    func: T,
    wait: number
) {
    let timeout: ReturnType<typeof setTimeout> | null = null;
    return function (...args: Parameters<T>): void {
        const later = () => {
            timeout = null;
            func(...args)
        }
        if (timeout !== null) {
            clearTimeout(timeout)
        }
        timeout = setTimeout(later, wait)
    }
}
```

# Debugging
- A função acima recebe uma outra função como parâmetro (func) e o tempo que queremos aguardar (wait).
- A função que passamos como parâmetro será executada depois que o tempo de aguardo finalizar dentro de ```later```.
