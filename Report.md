# Отчёт о тестировании приложения "Money Transfer"

## Краткое описание

Для определения ошибки в работе программы "Money Transfer" на основе входных данных был написан код Java-приложения, позволяющего воспроизвести ошибку. Было проведено тестирование кода приложения "Money Transfer" путём запуска программы и сравнения фактического результата работы программы с ожидаемым. Результаты тестирования показали, что программа работает некорректно, следовательно, в программе присутствует баг. После его идентификации все подробности были описаны в соотвествущем баг-репорте.

## Описание тестов

Проводилось функциональное тестирование позитивного сценария на основе входных данных: проверялась функция программы "Money Transfer" корректно учитывать изменение баланса банковского счёта, содержащего 2 000 000 000 (два миллиарда) рублей, при пополнении данного счёта на 500 000 000 (пятьсот миллионов) рублей.

## Результаты

1. Единственный проведённый тест был неуспешным. Программа не прошла проверку на соответствие заявленным требованиям.
2. Ссылка на баг-репорт: [Неверный результат при пополнении баланса счёта в Money Transfer](https://github.com/Filosoff42/JavaHW3-MoneyTransfer/issues/1#issue-788916225)

## Общие рекомендации
По условиям задания не нужно было досконально разбираться в причинах возникновения ошибки, однако я могу порекомендовать автору первоначального кода вспомнить, что максимальное значение для переменных типа `int` (integer) равняется 2 147 483 647.