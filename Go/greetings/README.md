## Tutorial: Create a Go module

- Go code is grouped into **packages**, and packages are grouped into **modules**
- Your module specifies dependencies needed to run your code, including the **Go version** and **the set of other modules it requires**

### greetings.go
- In Go, a function whose **name starts with a capital letter** can be called by a function **not in the same package**
![img.png](img.png)
- The `:=` operator is a shortcut for **declaring** and **initializing** a variable in one line

#### `Sprintf` function
```go
var message string
message = fmt.Sprintf("Hi, %v. Welcome!", name)
```
- The first argument is a **format string**, and Sprintf substitutes the name parameter's value for the `%v` format verb