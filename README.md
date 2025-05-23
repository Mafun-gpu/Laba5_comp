**Постановка задачи**

Целью данной лабораторной работы является расширение функциональности синтаксического анализатора, разработанного ранее, за счет включения этапа построения внутреннего представления программы в виде тетрад.В процессе выполнения работы необходимо реализовать разбор выражений по заданной контекстно-свободной грамматике методом рекурсивного спуска, проверку на лексические и синтаксические ошибки, а также генерацию тетрад с указанием операций и аргументов выражений.

**Вариант задания**

2 вариант. В качестве внутренней формы представления программы выберем тетрады. Тетрада имеет четыре поля: op, arg1, arg2 и result.

Задание:

1) Реализовать в текстовом редакторе поиск лексических и синтаксических ошибок для грамматики G[<E>]. Реализовать данную КС-граммматику методом рекурсивного спуска:
```
1. E → TA 

2. A → ε | + TA | - TA 

3. T → ОВ 

4. В → ε | *ОВ | /ОВ 

5. О → id | (E) 

6. id → letter {letter}
```
2) Реализовать алгоритм записи выражений в форме тетрад.

**Примеры верных строк**

```python
a + b
```
```python
x * y + z
```
```python
x + y * (a - b)
```
```python
a / (b + c)
```
```python
var1 * (var2 + var3) - var4
```

**Тестовые примеры**

![image](https://github.com/user-attachments/assets/b935319b-bfad-4d7d-948d-9f27d65742aa)
![image](https://github.com/user-attachments/assets/b1007736-6fc4-4a2f-b319-58e555e8b5f6)
![image](https://github.com/user-attachments/assets/a494ea18-5a65-43ac-af79-61e8fb47daa0)

