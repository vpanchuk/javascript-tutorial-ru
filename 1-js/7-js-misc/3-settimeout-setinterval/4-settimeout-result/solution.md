Ответы:

- `alert` выведет `100000000`.
- **3**, срабатывание будет после окончания работы `hardWork`.

Так будет потому, что вызов планируется на `100 мс` от времени вызова `setTimeout`, но функция выполняется больше, чем `100 мс`, поэтому к моменту ее окончания время уже подошло и отложенный вызов выполняется тут же.