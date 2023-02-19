## [Call your code from another module](https://go.dev/doc/tutorial/call-module-code)

### `go mod edit`
- Use the `go mod edit` command to edit the **example.com/hello** module to redirect Go tools from its module path (where the module isn't) to the local directory (where it is)
- `go mod edit -replace example.com/greetings=../greetings`

### go.mod
```go
require example.com/greetings v0.0.0-00010101000000-000000000000
```
- The number following the module path is a **pseudo-version number** -- a generated number used in place of a semantic version number (which the module doesn't have yet)