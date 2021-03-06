# AuraIncrementor
[![Build Status](https://app.bitrise.io/app/522240cc0369fafb/status.svg?token=R3GjZdH7cD0IUOUwqgORng&branch=master)](https://app.bitrise.io/app/522240cc0369fafb) [![codecov](https://codecov.io/gh/AgapovOne/AuraIncrementor/branch/master/graph/badge.svg)](https://codecov.io/gh/AgapovOne/AuraIncrementor)

Incrementor class. Fully tested framework &amp; pod

---

## How to use

To try:
`pod try AuraIncrementor` or download and open .xcodeproj :)

Cocoapods. Add to Podfile:
```
  pod 'AuraIncrementor'
```

#### Notes:

Internal interface is covered in public tests, but not tested itself with different inputs and constants.
`Incrementor.Constants` is introduced for easier support and extendability of an `Incrementor` class

---

## Задача для SWE - Basic

Нужно написать класс на Java/Swift/Golang/С (Си) со следующим интерфейсом (псевдокод):

```
class Incrementor {
  /**
   * Возвращает текущее число. В самом начале это ноль.
   */
  int getNumber();

  /**
   * Увеличивает текущее число на один. После каждого вызова этого
   * метода getNumber() будет возвращать число на один больше.
   */
  void
incrementNumber();
  /**
   * Устанавливает максимальное значение текущего числа.
   * Когда при вызове incrementNumber() текущее число достигает
   * этого значения, оно обнуляется, т.е. getNumber() начинает
   * снова возвращать ноль, и снова один после следующего
   * вызова incrementNumber() и так далее.
   * По умолчанию максимум -- максимальное значение int.
   * Если при смене максимального значения число резко начинает
   * превышать максимальное значение, то число надо обнулить.
   * Нельзя позволять установить тут число меньше нуля.
   */
  void setMaximumValue(int maximumValue);
}
```

Т.е. класс очень простой. А теперь сложность: оно должно быть сделано очень хорошо. Т.е. максимально качественно, как только можно. Код должен быть идеальным, все должно быть покрыто unit тестами. Классы и все методы должны быть полностью покрыты понятной (т.е. полезной, а не для отписки) javadoc (для Java) или аналогом для Swift и Golang документацией. В общем, нужно сделать такой код, который каждый разработчик мечтает получить на поддержку -- идеальный (насколько кандидат способен).

Обратить внимание на:
- Форматирование кода.
- Нэйминг (названия всех сущностей).
- Покрытие тестами.
- Наличие документации.
- Общая читабельность и простота кода.
В идеале результат можно предоставить в виде скрытого gist-а на gist.github.com.
