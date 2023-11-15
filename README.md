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
- [Что такой SOLID?](#)
- [**S - Single-responsibility principle**](#)
- [**O - Open-closed principle**](#)
- [**L - Liskov substitution principle**](#)
- [**I - Interface segregation principle**](#)
- [**D - Dependency Inversion Principle**](#)

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

## Что такой SOLID?

**SOLID** это набор принципов, следуя которым, программный код будет более чистым и гибким. Т.е. это не какае-то библиотека или технология, это просто правила, которым должен следовать любой адекватные разработчик, не зависимо на чем он программирует.
