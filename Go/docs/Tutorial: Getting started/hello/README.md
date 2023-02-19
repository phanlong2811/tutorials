## [Tutorial: Get started with Go](https://go.dev/doc/tutorial/getting-started)
### Enable dependency tracking
When import **packages** contained in **other modules**, you manage **those dependencies** through your code's own module.

#### go.mod
- File that **tracks the modules** that provide **those packages**

#### Command
- Run `go mod init example/hello` to enable **dependency tracking**
- `example/hello` is name of the module your code will be in
- In **actual development**, the module path will typically be the **respository location**

### hello.go
#### Run code
- `go run .`

#### `fmt` package
-  Contains functions for _formatting text_, including _printing to the console_
-  One of the **standard library** packages

### Call code in an external package
When you need to do something that might have been **implemented by someone else**, you can look for a package that has functions you can use in your code

#### `go mod tidy`
- Go will add the **quote** module as a requirement
- **go.sum** file for use authenticating the modules
- When you ran `go mod tidy`, it **located** and **downloaded** the _"rsc.io/quote"_ module that contains the package you imported.
