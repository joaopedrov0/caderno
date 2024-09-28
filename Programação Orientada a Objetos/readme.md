# Classes

O conceito de classes é algo fundamental para o entendimento de Orientação a Objetos. Trata-se de um modo mais estruturado de criar objetos na programação.

Em python a criação de uma classe se dá da seguinte forma:

```python
class NomeClasse: # Nome da classe com primeira letra maiúscula por convenção.

    lorem = "ipsum" # Exemplo de atributo de de classe

    # Construtor da classe
    def __init__(self, argumento1, argumento2, argumentoN):
        self.atributo1 = argumento1
        self.atributo2 = argumento2
        self.atributoN = argumentoN

    # Método de instância da classe (método que é dos objetos da classe)
    def metodoInstancia(self, bar):
        return foo(bar)

    # Método de classe
    @classmethod
    def metodoClasse(cls, bar):
        return foo(bar)

    # Método Estático
    @staticmethod
    def metodoEstatico(bar):
        return foo(bar)
```

... colocar explicação a respeito de classes com exemplos também

## Atributos de Classe

Atributos variáveis pertencentes a classe e compartilhados entre todas as instâncias. Uma alteração em um atributo de classe feito por uma instância vai mudar esse valor para TODAS as instâncias dessa classe.

```python
class Example:
    foo = "bar"
```

## Métodos de Classe

Métodos compartilhados entre todas as instâncias e que podem ser usados para manipular atributos de classe mencionados anteriormente. Recebem `cls` como argumento padrão para se referir à classe dentro do contexto do método da classe. Usa-se o decorador `@classmethod` para identificar um método de classe.

```python
class Example:
    @classmethod
    def exampleMethod(cls, bar):
        foo()
        return bar
```

## Métodos Estáticos

Métodos que não acessam o escopo nem de classe, nem de instância de classe. São referenciados com o decorador `@staticmethod` para simbolizar um método estático.

```python
class Example:
    @staticmethod
    def exampleStaticMethod():
        foo()
        return bar
```

> ## Cuidado!
> Em outras linguagens, é comum usar a palavra chave `static` para referenciar atributos e métodos de classe. Em python, métodos estáticos são algo à parte, são métodos usados fora de contexto e que podem ser usados para testes.

## Instâncias de Classe

Instâncias de classe são objetos gerados com base nas "regras" de uma classe. Instâncias de objeto geradas por uma classe terão todos os métodos e atributos que a definição da classe disser que ela terá.

Observe o exemplo abaixo:

person.py
```python 
class Person:
    race = "human"
    def __init__(self, name, age):
        self.name = name
        self.age = age
```

main.py
```python
from person.py import Person

kaira = Person("Kaira", 23)
```

No exemplo anterior o código no arquivo `main.py` vai armazenar na variável `kaira` um objeto que contém os atributos `name`, `age` e `race`. E qualquer outra instância vai ter estes três atributos com os valores especificados na instanciação do objeto, e o valor fixo `"human"` para o atributo de classe `race`

## Construtor

### Atributos de instância de Classe

Atributos distribuídos entre todas as instâncias de objetos da classe. Recebem valores independentes para cada instância gerada pela classe e sua alteração não afeta os demais.

### Métodos de instância de Classe

Métodos distribuídos entre todas as instâncias de objetos da classe. Recebem a palavra chave `self` para se referir ao objeto.


# Relação de Classes

> ## Tipos de relações entre classes
> - Associação
> - Herança
> - Interface
> - Agregação
> - Composição

## Associação de Classes

...

explicar melhor depois !

mas basicamente oq ele fala é de uma classe que usa uma instância de outra classe tlgd
tipo, uma classe pessoa que tem um metodo que depende de uma classe interruptor pra conseguir apagar a luz