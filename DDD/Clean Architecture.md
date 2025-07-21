## Clean Architecture
- Ver [essa](https://blog.cleancoder.com/uncle-bob/images/2012-08-13-the-clean-architecture/CleanArchitecture.jpg) imagem
- Princípio de desacoplamento: Permite com que cada parte do nosso software não esteja totalmente acoplada a uma camada externa (infraestrutura)
- Infraestrutura: Camada onde não temos muito controle, como banco de dados, parte de interação com o usuário (Frameworks and drivers)
- Interface Adapters: Fará a adaptação dos dados para as camadas mais internas, além de proteger esses dados.
- "Flechas": Representam a dependência entre as camadas (As entidades não podem importar nada de use-cases, mas use-cases podem importar de entidades). Elas também podem representar o fluxo.

**Se usarmos os princípios corretos do Clean Architecture, as últimas duas camadas (use cases e entities) poderão ser passadas para outros frameworks, e isso não afetará o funcionamento.**
