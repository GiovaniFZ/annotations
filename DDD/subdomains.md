## Subdomínios
- **Tudo o que toca a lógica do problema que estamos resolvendo pode ser um subdomínio**
- **Os subdomínios precisam se comunicar entre si**
- **Não é necessário separar entre microsserviços, ou sistema de mensageria. Mesmo assim é importante não criar dependencias de código entre os subdomínios.**

## Tipos
- Core: O que dá dinheiro (monetário)
- Supporting: Dá suporte para o core funcionar
- Generic: Precisa deles mas são menos importantes.

## Exemplos

### Core: 
- Compra
- Catálogo
- Pagamento
- Entrega.

### Supporting
- Estoque
  
### Generic
- Notificação
- Promoções
- Chat
