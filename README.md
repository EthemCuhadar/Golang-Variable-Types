# Golang

![Golang Image](golang.png)

-------------------------------------------------------------------

## General Information

- **Golang**, aka "**Go**", is an open source, statically typed and compiled programming language designed at Google by ***Robert Griesemer***, ***Rob Pike*** and ***Ken Thompson***. 

- Go was publicly announced in Novermber 2009. 

- General usage areas of the language are ***Cloud Computing*** and ***Web Applications and Services***.

--------------------------------------------------------

## Getting started with "Hello World"

Our first program will print "Hello World". The code is shown below. 

```go
package main

import "fmt"

fun main(){
    ftm.Println("Hello World")

}
```

To run the code, type "go run filename.go" in terminal. 

```console
go run hello-world.go
Hello World
```

--------------------------------------------------------------------

# Starting with Variable Types

* In Go, "var" declares variables.
* In Go programming language, several variables can be defined in single line as shown below.

```go
var intVal1, intVal2 int = 10, 20
```

```go
var intVal, strVal = 10, "patika"
```

--------------------------------------------------------

## Booleans

Boolean data type is the data type which can be ***True*** or ***False***. Example code is shown below.

```go
package main

import "fmt"


fun main(){

    var boolVal1 bool
    fmt.Println(boolVar1)

    var boolVal2 = true
    fmt.Println(boolVal2)
}
```

```console
go run Booleans.go
false
true
```

* Default bool value in Go is false
* When boolVal2 is pointed to ***true***, it is not necessary to decleare type bool.

-------------------------------------------------------

## Integers

There are 4 types of integers in Go which are **int8**, **int16**, **int32** and **int64**.

```go
package main

import (
    "fmt"
    "reflect"
)

func main() {

    var intVal1 int8 = 10
    var intVal2 int16 = 10

    fmt.Println(intVal1)
    fmt.Println(intVal2)

    fmt.Printf("Type of intVal1: %v\n", reflect.TypeOf(intVal1))
    fmt.Printf("Type of intVal2: %v\n", reflect.TypeOf(intVal2))

}
```

```console
10
10
Type of intVal1: int8
Type of intVal1: int16
```

In Go programming language, variable types are very strict. Therefore, you cannot apply basic operations for different types of variables such as adding and multiplication. You can see an example of this situation below with decleared values of ***intVal1*** and ***intVal2***.

```go
fmt.Println(intVal1 + intVal2)
```

```console
# command-line-arguments
.\Integers.go:25:22: invalid operation: intVal1 + intVal2 (mismatched types int8 and int16)
```

* The general types of these 2 values may be the same. However, there are also 4 types in the integers. Hence, integer types are different for this situation.

--------------------------------------------

## Floats

There are 2 types of floats in Go programming language which are ***float32*** and ***float64***. Likewise integers, the types of these two are different. Therefore, the operations between these 2 types of floats will cause an error.

```go
package main

import (
    "fmt"
    "reflect"
)

func main() {

    var floatVal1 float32 = 10.2
    var floatVal2 float64  = 10.2

    fmt.Println(floatVal1)
    fmt.Println(floatVal2)

    fmt.Printf("Type of floatVal1: %v\n", reflect.TypeOf(floatVal1))
    fmt.Printf("Type of floatVal2: %v\n", reflect.TypeOf(floatVal2))

}
```

```console
10.2
10.2
Type of floatVal1: float32
Type of floatVal2: float64
```

--------------------------------------------------------------

## Strings

String is one of the main types in Go programming language like other programming languages, Java, Python, C++. There are no different types of strings. Therefore, all strings are same type of variables. Some operations like concatenate can be applied between string variables.

```go
package main

import (
    "fmt"
    "reflect"
)

func main() {

    var strVal1 string = "patika"
    var strVal2 string = "bootcamp"


    fmt.Println(strVal1)
    fmt.Println(strVal2)

    fmt.Printf("Type of the strVal1 is: %v\n", reflect.TypeOf(strVal1))
    fmt.Printf("Type of the strVal2 is: %v\n", reflect.TypeOf(strVal2))

    fmt.Println(strVal1 == strVal2, " if they are equal")
    fmt.Println(reflect.TypeOf(strVal1) == reflect.TypeOf(strVal2), " if they are same type")

    fmt.Println(strVal1 + " " + strVal2)
}
```

```console
patika
bootcamp
Type of the strVal1 is: string
Type of the strVal2 is: string
false  if they are equal
true  if they are same type
patika bootcamp
```

-------------------------------------------------
