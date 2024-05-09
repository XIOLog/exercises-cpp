Представим себе, что мы пишем программу которая принимает из консоли возраст пользователя и выводит его на экран:

```cpp
#include <iostream>

int main() {
  int user_age { 0 };
  std::cout << "Enter your age: " << std::endl;
  std::cin >> user_age; // объект cin отвечает за стандартный ввод
  std::cout << user_age << std::endl;
}
```

Давайте изменим название переменной `user_age`:

```cpp
int main() {
  int x { 0 };
  std::cout << "Enter your age: " << std::endl;
  std::cin >> x; // объект cin отвечает за стандартный ввод
  std::cout << x << std::endl;
}
```

Она по прежнему работает, но в ней изменилось имя переменной на `x`. Компьютеру без разницы, как мы называем переменные, это бездушная машина, но вот программистам — нет. Мы гораздо чаще читаем код, чем пишем. Причём не свой, а написанный другими людьми. От качества и понятности имён переменных зависит половина успеха в анализе кода.

Лучше посидеть и придумать название, которое описывает суть, смысл переменной, чем назвать её как попало, а в будущем переделывать. Постарайтесь давать им такие имена, чтобы они были максимально понятны без контекста, без изучения окружающего кода.

Существует общепринятое правило: не используйте транслит для имён, только английский язык. Если вы испытываете сложности с английским, то пользуйтесь переводчиком. Со временем, копаясь в чужом коде, вы сформируете правильные понятия для именования.

Среди разработчиков есть шутка: «самое сложное в программировании — названия переменных и инвалидация кеша». Придумывать названия и правда сложно. Как бы вы назвали переменную, в которой хранится _количество неоплаченных заказов от клиентов, имеющих задолженность в предыдущем квартале?_

Самопроверка. Придумайте название для переменной, в которой будет храниться _«количество пользователей не совершавших покупки»_. Запишите его в блокноте или отправьте себе на почту. Не указывайте там ничего, кроме названия переменной. А через несколько уроков мы вернёмся к этой теме ;-)