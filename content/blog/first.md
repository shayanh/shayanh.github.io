---
title: "First"
date: 2020-02-13T16:34:03+03:30
draft: true
---

This is the first post.

```go
package main

import "fmt"

func main() {
    ch := make(chan float64)
    ch <- 1.0e10    // magic number
    x, ok := <- ch
    defer fmt.Println("exitting now")
    go println(len("hello world!"))
    return
}
```
