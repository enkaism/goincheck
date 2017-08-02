# goincheck
coincheck client API for golang

# Installation

```
$ go get github.com/takuyaohashi/goincheck
```

# Usage Example
```
package main

import (
    "fmt"

    "github.com/takuyaohashi/goincheck"
)

const (
    accessKey       = "hoge"
    secretAccessKey = "huga"
)

func main() {
    client, _ := goincheck.NewClient(accessKey, secretAccessKey)
    tikcer, _ := client.GetTicker()
    fmt.Printf("Tikcer = %+v\n", tikcer)
}
```

For detail, please check ``sample/cmd/`` directory.

# License
MIT
# Author
Takuya OHASHI
