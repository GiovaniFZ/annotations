# DDD: Domain Driven Design
- Design dirigido a domínio
- Domínio: Problema que estamos resolvendo
- Não está relacionado em como que vamos estruturar nosso projeto, em pastas ou arquivos
- Está relacionado em como vamos converter o problema do nosso cliente em algo palpável.
- DDD: Desenho da aplicação, é pensar em quais entidades existiram na aplicação a nível de design
- Não é uma arquitetura, mas sim um passo antes.
## Domínio
- Entende-se como uma área de entendimento, onde todas as pessoas no desenvolvimento possuem pensamentos parecidos.
## Subdomínios
- Processos que acontecem dentro da problemática que queremos resolver
- Diferentes áreas de entendimento dentro de um domínio maior
## Entidades
- "Atores" dentro dos nossos subdomínios
- **Uma mesma possível entidade pode ter nomes diferentes**
- Exemplo: um user pode ser um cliente, um destinatário, etc.
## Domain Experts
- Experts de domínio são pessoas que entendem, a fundo, a problemática que estamos resolvendo com nosso softwares. (Pessoas de negócio)
- Ou seja, a conversa com os experts é fundamental.
- Exemplo: "Pegar as ordens de pedido e emitir as notas fiscais"
Caso de uso (ações): Emitir
Entidades: Ordens de pedido, notas fiscais
## Linguagem ubíqua
- Linguagem que todas as pessoas envolvidas conseguem conversar.
## Conceitos do DDD
- Agregados
- Value Objects
- Eventos de domínio
- Subdomínios (Bounded Contexts)
- Entidades, casos de uso
**Design de software é diferente de arquitetura de software!**