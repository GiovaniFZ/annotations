# SOLID
- S: Single Responsibility Principle: Uma classe ou módulo deve ter **apenas uma** razão para mudar.
- O: Open Closed Principle: Fechado para mudanças, aberto para adição de novas funcionalidades
- L: Liskov Substitution Principle: Se o programa usa uma classe base, deve ser possível substituir aquela classe com outra subclasse e isso não quebrará.
- I: Interface Segregation Principle: Uma classe não deve implementar métodos que ela não usa.
- D: Dependency Inversion Principle: Inverte a ordem de como a dependência é estabelecida.

## Cuidado
Esses princípios servem para ajudar a escrever um código melhor. Nada é essencial para escrever um código limpo no back end.

## Como saber se eu estou infringindo os princípios
**1. SRP**\
Vamos supor que há uma entidade que envia algo para o usuário **E** mostra uma tela de boas vindas. Isso não é correto, deve-se ter uma parte que envia algo e outra parte que mostra a tela de boas vindas.

**2. OCP**\
Quando eu tenho partes do meu código que tenham condicionais que facilmente teremos que adicionar ifs no futuro.
Exemplo: Calculo de fretes com vários ifs para cada transportadora

**3. LSP**\
Vamos supor que estamos trabalhando com um banco de dados X que possui métodos para CRUD. Ao alterar para outro banco que possa fazer a mesma coisa, a classe original que importa o repositório não deve parar de funcionar.

**4. ISP**\
Se tivermos uma interface gigante com várias propriedades juntas estamos infringindo o ISP.

**5. DIP**\
As dependências de uma classe devem ser injetadas (funcionalidades externas) dentro da classe.
No caso de funções, por exemplo, a dependência poderia ser passada como parâmetro.
