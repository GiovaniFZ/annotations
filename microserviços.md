# Microserviços
- Ideia: Separar o back end (que inicialmente pode ser monolítico) em vários que conversam entre si
- Normalmente em um BE monolítico, a conversa é feita por HTTP. Nos microserviços, além do HTTP também normalmente temos comunicação de eventos e mensageria.

| BE Monolítico | Microserviços |
| ------------- | -------------- |
| Centralizado  | Descentralizado |
| Mesmo BD      | BDs diferentes |
| Mesma linguagem | Linguagens agnósticas |
| Dependência de deploy | Independência de deploy |
| Requer menos experiência | Requer mais experiência |

# Vantagens e desvantagens - BE Monolítico
| Vantagens | Desvantagens |
| ------------- | ---------- |
| Fácil de desenvolver | Dificulta escalabilidade independente |
| Deploy facilitado | Falha em algum ponto afetará tudo |
|  Bom para MVP     | Tecnologia única para tudo |

# Vantagens e desvantagens - Microserviços
| Vantagens | Desvantagens |
| -------------- | -------------------|
| Escalabilidade independente | Complexidade de rede |
| Falhas isoladas | Debugging distribuído |
| Tecnologias diversificadas | Consistência entre eventos |

