# SOLID
- D: Dependency Inversion Principle: Inverte a ordem de como a dependência é estabelecida.
- O: Open Closed Principle: 
- L: Liskov Substitution Principle
- I: Interface Segregation Principle
- S: Single Responsibility Principle

## Cuidado
Esses princípios servem para ajudar a escrever um código melhor. Nada é essencial para escrever um código limpo no back end.

## Como saber se eu estou infringindo os princípios
1. SRP
Vamos supor que há uma entidade que envia algo para o usuário **E** mostra uma tela de boas vindas. Isso não é correto, deve-se ter uma parte que envia algo e outra parte que mostra a tela de boas vindas.

2. OCP
Quando eu tenho partes do meu código que tenham condicionais que facilmente teremos que adicionar ifs no futuro.
Exemplo: Calculo de fretes com vários ifs para cada transportadora

3. Liskov Substitution Principle
Vamos supor que estamos trabalhando com um banco de dados X que possui métodos para CRUD. Ao alterar para outro banco que possa fazer a mesma coisa, a classe original que importa o repositório não deve parar de funcionar.

4. Interface Segregation Principle
Separar as interfaces em mais interfaces.

5. Dependency Inversion Principle
As dependências de uma classe devem ser injetadas (funcionalidades externas) dentro da classe.
No caso de funções, por exemplo, a dependência poderia ser passada como parâmetro.
