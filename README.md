# Список вопросов на собеседовании JAVA

# CORE - 1

## ООП
- [Что такое ООП?](#что-такое-ооп-)
- [Какие преимущества у ООП?](#какие-преимущества-у-ооп-)
- [Какие недостатки у ООП?](#)
- [Назовите основные принципы ООП?](#)
- [Что такое инкапсуляция?(С примером)](#)
- [Что такое наследование?(С примером)](#)
- [Что такое полиморфизм?(С примером)](#)
- [Что такое абстракция?(С примером)](#)
- [Что такое ассоциация, агрегация и композиция?](#)
- [Расскажите про раннее и позднее связывание.](#)
## SOLID
- [Что такой SOLID?](#что-такой-solid)
- [**S - Single-responsibility principle**](#)
- [**O - Open-closed principle**](#)
- [**L - Liskov substitution principle**](#)
- [**I - Interface segregation principle**](#)
- [**D - Dependency Inversion Principle**](#)
## ООП в JAVA
- [1. Какие виды классов есть в java?](#)

## Что такое ООП? 🧠

Объектно-ориентированное программирование (ООП) — это подход, при котором программа рассматривается как набор объектов, 
взаимодействующих друг с другом. У каждого есть свойства и поведение. Если постараться объяснить простыми словами, то 
ООП ускоряет написание кода и делает его более читаемым.

## Какие преимущества у ООП? 🧠

- **Модульность:** Объектно-ориентированный подход позволяет сделать код более структурированным, в нем легко разобраться стороннему человеку. 
                   Благодаря инкапсуляции объектов уменьшается количество ошибок и ускоряется разработка с участием большого количества программистов, 
                   потому что каждый может работать независимо друг от друга.
- **Гибкость:**    ООП-код легко развивать, дополнять и изменять. Это обеспечивает независимая модульная структура. Взаимодействие с объектами, а не 
                   логикой упрощает понимание кода. Для модификации не нужно погружаться в то, как построено ПО. Благодаря полиморфизму можно быстро 
                   адаптировать код под требования задачи, не описывая новые объекты и функции.
- **Экономия времени:** Благодаря абстракции, полиморфизму и наследованию можно не писать один и тот же код много раз. Это ускоряет разработку нового ПО. 
                        Интерфейсы и классы в ООП могут легко преобразовываться в подобие библиотек, которые можно использовать заново в новых проектах. 
                        Также ООП экономит время при поддержке и доработке приложения.
- **Безопасность:** Программу сложно сломать, так как инкапсулированный код недоступен извне

## Какие недостатки у ООП? 🧠

- **Сложный старт:** Чтобы пользоваться ООП, нужно сначала изучить теорию и освоить процедурный подход, поэтому порог входа высокий.
- **Снижение производительности:** Объектно-ориентированный подход немного снижает производительность кода в целом. Программы работают несколько медленнее 
                                   из-за особенностей доступа к данным и большого количества сущностей.
- **Большой размер программы:**    Код, написанный с использованием ООП, обычно длиннее и занимает больше места на диске, чем «процедурный». Это происходит, 
                                    потому что в такой программе хранится больше конструкций, чем в обычном процедурном скрипте.
## Назовите основные принципы ООП. 🧠

Объектно-ориентированное программирование определяют через четыре принципа, по которым можно понять основы работы. Иногда количество сокращают до трех — опускают понятие абстракции.
- Абстракция
- Инкапсуляция
- Наследование
- Полиморфизм

## Что такое ассоциация, агрегация и композиция? 🧠
Композиция и агрегация являются частными случаями ассоциации.

- **Ассоциация** - это когда классы имеют ссылки друг на друга, так как им необходимо взаимодействовать между собой. Например, класс Собака и класс Человек. Оба являются независимыми, самодостаточными, но иногда они взаимодействуют между собой
- **Композиция** - это когда какой то класс является самодостаточным, а другие не могут независимо от него существовать. Например, класс Рука и класс Человек. Рука является частью Человека, но она не может существовать отдельно от Человека.
- **Агрегация** - аналогично композиции, но здесь уже класс является самодостаточным и он может быть использован в различных классах. Например, класс Телевизор и класс Бабушка и класс Дедушка. С Телевизором Бабушка и Дедушка могут выполнять различные действия, не обязательно что только один класс.

## Что такой SOLID? 🧠

**SOLID** - это набор принципов, следуя которым, программный код будет более чистым и гибким. Т.е. это не какае-то библиотека или технология, это просто правила, которым должен следовать любой адекватные разработчик, не зависимо на чем он программирует.

## S - Single-responsibility principle 🧠
Принцип единой ответственности означает, что один класс или файл должен иметь только одну цель и одно единственное назначение. Вы не имеете права создавать классы и файлы, которые представляют собой "комбайн" умеющий делать все.

Например, если ваш класс создан, что-бы отображать данные на экране, то не нужно размещать в этом классе логику получения этих данных из интернета.

Дело в том, что может получится ситуация, что меняя логику загрузки данных из интернета, вы случайно испортите логику отображения данных на экране. Поэтому работу с интернетом и отображением необходимо разделять на два разных класса.

Также, не забываем, что у вас есть интерфейсы и абстрактные классы, с помощью которых вы можете передавать интерфейс логики с интернетом, в класс для отображения. В итоге реализация интерфейса будет конкретная для конкретного случая, т.е. вам достаточно поменять реализацию интерфейса или абстрактного класса, если логика загрузки данных изменится.

Что-бы проверить, соответствует ли ваш класс этому принципу, задайте себе вопрос: Что может случится, из-за чего мне потребуется изменить данный класс?. Если ответов несколько, значит необходимо разделить класс на несколько.

## O - Open-closed principle 🧠

Принцип открытости/закрытости означает, что программные сущности(классы, интерфейсы и т. д.) должны быть открыты для расширения, но закрыты для модификации.

Например, у вас есть класс, который выполняет определенные функции. Если вам понадобилось добавить дополнительный функционал, то необходимо создать наследника этого класса или использовать композицию. Но, изменять исходный класс запрещено. Это необходимо, что-бы не испортить код, использующий этот класс.

В ряде случаев рекомендуется избегать наследования и применять композицию, что-бы избежать сложных структур данных и сделать код еще более независимым.

Одним словом, изменять код базового класса строго настрого запрещено!

## L - Liskov substitution principle 🧠

Принцип подстановки Барбары Лисков, самый не понятный принцип из-за названия :). Но все достаточно просто и немного похоже на предыдущий принцип. Принцип гласит, что поведение методов в дочернем классе должно следовать принципам базового класса, а не изменять их. То есть, дочерний класс переопределяя методы или переменные, не должен менять заложенную логику базового класса.
**Пример**
```java
public class Rectangle {
  private int width;
  private int height;

  public int getWidth() {
    return this.width;
  }

  public int getHeight() {
    return this.height;
  }

  public void setWidth(int width) {
    this.width = width;
  }

  public void setHeight(int height) {
    this.height = height;
  }
}

public class Square extends Rectangle {
  public void setSize(int size) {
    super.setWidth = size;
    super.setHeight = size;
  }
}
```

Выглядит немного странно, правда? Класс Square(Квадрат) наследуется от Rectangle(прямоугольник), а так как у квадрата все стороны равны, в классе Square мы просто задаем ширину и высоту, одну и ту же. В итоге, мы испортили изначальную идею класса Rectangle, в который заложена логика, что стороны могут отличаться. Получается, не меняя базовый класс, мы умудрились нарушить данный принцип.

В этом примере Square должен быть отдельным классом и ни в коем случае не наследоваться от Rectangle. То есть, поведение методов не должно изменяться. Если написано, что метод возвращает ширину, значит он и должен возвращать ширину, а не что-то другое.

## I - Interface segregation principle 🧠

Принцип разделения интерфейса. Тут все очень просто. Лучше создавать много отдельных узкоспециализированных интерфейсов, чем один, который включает в себя много функций. Это позволит сделать архитектуру более гибкой, и позволит использовать интерфейсы по отдельности. Этот принцип похож на самый первый, принцип единой ответственности.

Пример:
```java
interface ItemClick {
  void onClick();
  void onLongClick();
}
```
Итак, есть интерфейс, который требует реализовать два метода: короткое нажатие и длинное нажатие. Но что, если нам необходимо только короткое нажатие? В этом случае у нас будет, что-то такое:
```java
public class MyClass implements ItemClick {
  void onClick() {
    // тут реализуем необходимую логику
  }
  coid OnLongClick() {
     // а вот тут нам нечего не надо делать, но все равно приходится
     // реализовать этот метод потому, что этого требует интерфейс
  }
}
```

Что-бы этого избежать необходимо сделать два разных интерфейса, которые можно применять по отдельности.

```java
interface ItemClick {
    void onClick()
}
interface ItemLongClick {
    void onLongClick()
}
```
Мы создали новый интерфейс, вместо того, чтобы расширять существующий. Это позволяет использовать эти интерфейсы, как отдельно, так и вместе, что делает архитектуру более гибкой и изменяемой. Если бы мы создали новый метод в существующем классе, то нам пришлось бы реализовать его в классе, который его уже использует, а это значит, мы вмешиваемся в существующий код.

```java
class Main {
  public static void main(String ....args) {
    System.out.println("Hello world!");
  }
}
```

```C++
#include <iostream>

int main() {
    std::cout << "Hello World!";
    return 0;
}
```

```python
print("Hello world!")
```







