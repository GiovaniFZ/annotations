# Pilares da programação orientada a objetos

## 1. Herança
É a capacidade de uma classe A herdar métodos e atributos de uma classe B.
Exemplo:
```csharp
public ClassB {
    // atributos e métodos de B
}

public ClassA: ClassB {
    // atributos e métodos de A
}
```

## 2. Encapsulamento
É a capacidade de uma classe, e seus métodos possuirem modificadores de acesso, permitindo o controle sobre os dados. Em C#, existem 2 modificadores de acesso para classe: internal e public. Atributos e métodos adicionam protected e private. Um detalhe é que se por exemplo tivermos 2 projetos P1 e P2 e se P2 possui permissão para ver as classes de P1, então P1 não pode ter permissão para ver as classes de P2, pois isso gera dependência cíclica.
**Modificadores**
1. Internal: Só funciona dentro de um projeto específico
```csharp
public class ClassProjectA {
    public void AnyFunction() {
        var instance = new ClassProjectB() // Resultará em erro
    }
}

internal class ClassProjectB {
    /*
    Essa classe pertence apenas ao projeto B
    */
}
```
2. Private: Atributos e métodos não podem ser acessados por nenhuma classe, independente do projeto. Para poderem acessar, precisa de um getter e para modificar, um setter.
```csharp
public class MyClass {
    private string Nome { get; set; }
}
```

3. Protected: Se uma classe A herda de B, e C herda de B porém métodos de A são protected, C não consegue ter acesso nesses métodos.
```csharp
public class ClassA {
    protected string Name { get; set; }
}
public class ClassB: ClassA {
    // Classe B pode 
}
public class ClassC {
    public void MyFunction() {
        var instance = new ClassB()
        var name = instance.Name; // Ocorrerá erro
    }
}
```

# 3. Abstração
Quando uma classe é marcada como abstrada, ela não poderá ser instanciada. Útil se ela for genérica. Métodos marcados como abstract preciam ser instanciados obrigatoriamente.
# 4. Polimorfismo
Polimorfismo significa várias formas, ou seja, se uma classe A herda métodos e atributos de B, a classe A também pode ser chamada de B.
```csharp
public abstract class Automobile {
    public string Color { get; set; }
    public string Model { get; set; }
    public void DoAnything() {}
}

public class Car : Automobile {

}

var car = new Car();
AnyFunction(car)

public void AnyFunction (automobile Automobile) {
    automobile.DoAnything() // Deve funcionar
}

```