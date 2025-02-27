## Buffer
- Definição: É uma representação de um espaço da memória do computador. 
- São usados para transitar dados de forma rápida
- São dados binários, não é bem suportado pelo JavaScript

```
const buf = Buffer.from("ok")
console.log(buf) -> <Buffer 6a 6b>
```