# Babel
- É um "transpilador" (conversor) de JavaScript
- Ou seja, ele é responsável por transformar (converter) um JSX em algo que o browser entende.
# Exemplo:
```ts
function MyComponent() {
    return <h1>Test</h1>
}
```
- Esse componente será convertido pelo Babel em algo como:
```ts
import { jsx as _jsx } from 'react/jsx-runtime'
function MyComponent() {
    return _jsx("h1", {
        children: "Test"
    });
}
```
