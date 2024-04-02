# Средства отладки IntelliJ IDEA
## Точки прерывания

Точки прерывания (останова) служат для выполнения программы до заданной строки с точкой, с целью просмотра и анализа кода программы.

Точки прерывания в IntelliJ устанавливаются нажатием  левой клавишей мыши на поле с номерами строк (слева).

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/2c13b008-1f02-4886-985f-ef338d857833)


Работа с точками останова возможна только в режиме отладки.

Войти в режим отладки можно нажав Shift-F9

Двигаться вниз по строкам, выполняя инструкции программы и просматривая результат выполнения отладочном коне внизу экрана
можно с помощью клавиши F8.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/b36776cf-e8f9-4ab6-8ac9-8330f4ab2ef6)

При наведении курсора мыши на точку останова открыввается меню, где можно ввести условия останова программы в данной точке, отключить или включить опять точку прерывания.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/26a052fd-eee9-4800-a370-393fccd939be)


## Инструкция утверждения assert

Assert требует для продолжеиня работы программы верный результат выполнения своего условия. 
Если результат верен (принимает логическое значение true), то программа двигается дальше.

Если же ожидание оказывается ложным, то программа завершится исключением типа AssertionError.

В приведенном ниже примере не прошло проверку условие выбора позиции в строке:

assert pos >= 0;         // test assert 2

assert pos < len1 -1;

Позиция оказалась больше чем длина строки, минус 1.

Результатом будет выход в исключение  AssertionError.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/d1eef0c2-c6d2-4f3e-b397-c64126ac927a)

Для более подробной информации, при выходе в данный тип исключений, можно с помощью несложного синтаксиса, вывести результат выполнеиня assert.

После двоеточия необходимо записать информацию для ввывода на экран.

 assert pos + len2 <= len1 : "Длина подстроки = " + (pos + len2);
 
Результат:  Длина подстроки = 104, что и привело к выходу в исключение.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/5d310f02-7eb8-42e7-9906-a9b56cec4fa2)

Необходимо отметить, что по умолчанию в пакете IntelliJ выключена обработка assert по умолчанию. 

Включить ее можно в меню EditConfiguration.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/75d94538-4630-4037-ab96-ab5d462b30f1)

Для этого в поле arguments для проекта и для VM нужно ввести -ea:

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/c068953b-4033-4ec7-b061-6be4e74e0de9)

