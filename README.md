## go-strftime [![Build Status](https://travis-ci.org/acstech/go-strftime.svg)](https://travis-ci.org/acstech/go-strftime)

Go date time format compatible with Ruby's [Time#strftime](http://ruby-doc.org/core-2.2.2/Time.html#method-i-strftime)


## Install
go get github.com/acstech/go-strftime


## Example

```go
package main

import (
  "fmt"
  "time"

  "github.com/acstech/go-strftime"
)

func main() {
  t := time.Now()
  s := strftime.Strftime(&t, "%Y-%m-%d %H:%M:%S")
  fmt.Println(s)
}
```
