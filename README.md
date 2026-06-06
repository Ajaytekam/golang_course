## Usage: 


Create a package

```
go mod init example/hello
```

Edit go.mod and add the require statement with the package repo url and also mention latest keyword

```
module example/hello2

go 1.25.1

require github.com/ajaytekam/golang_course latest
```

Create main.go and run the command `go mod tidy` it will download the pcakage from github.

Edit main.go and put below code

```
package main

import "github.com/ajaytekam/golang_course"

func main() {
	golang_course.SayHello01()
	golang_course.SayHello02()
}
```



