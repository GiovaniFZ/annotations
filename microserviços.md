# Microserviços
- Ideia: Separar o back end (que inicialmente pode ser monolítico) em vários que conversam entre si
- Normalmente em um BE monolítico, a conversa é feita por HTTP. Nos microserviços, além do HTTP também normalmente temos comunicação de eventos e mensageria.

| BE Monolítico | Microserviços |
| ------------- | -------------- |
| Centralizado  | Descentralizado |
| Mesmo BD      | BDs diferentes |
| Mesma linguagem | Linguagens agnósticas |
| Dependência de deploy | Independência de deploy |
