# Средства отладки IntelliJ IDEA
## Точки прерывания
Точки прерывания служат для выполнения программы до заданной строки с точкой, с целью просмотра и анализа кода программы.

Точки прерывания в IntelliJ устанавливаются нажатием  левой клавишей мыши на поле с номерами строк (слева).

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/2c13b008-1f02-4886-985f-ef338d857833)


Работа с точками останова возможна только в режиме отладки.

Войти в режим отладки можно нажав Shift-F9

Двигаться вниз по строкам, выполняя инструкции программы и просматривая результат выполнения отладочном коне внизу экрана
можно с помощью клавиши F8.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/b36776cf-e8f9-4ab6-8ac9-8330f4ab2ef6)

При подведении мыши открыввается ниспадающее меню, где можно ввести условия останова программы в данной точке, отключить и включить опять точку останова.

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/26a052fd-eee9-4800-a370-393fccd939be)


## Инструкция утверждения assert
Assert верный результат предыдущего действия. Если результат верен (принимает логическое значение true), то программа двигается дальше.
Если же ожидание оказываетс яложным, то программа завершится исключением типа AssertionError.

В приведенном ниже примере 
![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/d1eef0c2-c6d2-4f3e-b397-c64126ac927a)

![image](https://github.com/SvetlanaBoichenko/JavaDebug/assets/160069590/5d310f02-7eb8-42e7-9906-a9b56cec4fa2)


