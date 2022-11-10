# 1. 介绍

## 1.1 安装

## 1.2 交互模式

## 1.3 运行脚本

```elixir
iex> elixir simple.exs
```

# 2. 基本类型

```elixir
iex> 1          # integer
iex> 0x1F       # integer
iex> 1.0        # float
iex> true       # boolean
iex> :atom      # atom / symbol
iex> "elixir"   # string
iex> [1, 2, 3]  # list
iex> {1, 2, 3}  # tuple
```



## 2.1 基本算法

```elixir
iex> 1 + 2
3
iex> 5 * 5
25
#请注意，它10 / 2返回了一个浮点数5.0而不是一个整数5。这是意料之#中的。在 Elixir 中，操作符/总是返回一个浮点数。如果要进行整数
#除法或得到除法余数，可以调用divandrem函数：
iex> 10 / 2
5.0
iex> div(10, 2)
5
iex> div 10, 2
5
iex> rem 10, 3
1
#Elixir 还支持用于输入二进制、八进制和十六进制数字的快捷符号：
iex> 0b1010
10
iex> 0o777
511
iex> 0x1F
31
#浮点数需要一个点后跟至少一位数字，并且还支持e科学记数法：
iex> 1.0
1.0
iex> 1.0e-10
1.0e-10
#您可以调用该round函数来获取与给定浮点数最接近的整数，或者调用该函数来获取浮点数trunc的整数部分。
iex> round(3.58)
4
iex> trunc(3.58)
3
```



## 2.2 识别功能和文档

```elixir
#Elixir 中的函数由它们的名称和数量来标识。函数的arity 描述了函数采用的参数的数量。从这一点开始，我们将在整个文档中使用函数名称及其数量来描述函数。trunc/1标识命名trunc并接受1参数的函数，而trunc/2标识具有相同名称但元数为 的不同（不存在）函数2。

#我们也可以使用这种语法来访问文档。Elixir shell 定义了h函数，您可以使用它来访问任何函数的文档。例如，输入h trunc/1将打印trunc/1函数的文档：
iex> h Kernel.trunc/1
                             def trunc()

Returns the integer part of number.
```



## 2.3 布尔值

```elixir
iex> true
true
iex> true == false
false
iex> is_boolean(true)
true
iex> is_boolean(1)
false
#您还可以使用is_integer/1,is_float/1或is_number/1分别检查参数是整数、浮点数还是其中之一
```



## 2.4 原子

## 2.5 字符串

## 2.6 匿名函数

## 2.7 （链接）列表

## 2.8  元组

## 2.9  列表还是元组？

