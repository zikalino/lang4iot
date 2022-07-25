# TinyGo

## Example

    docker build --tag lang4iot/go .
    
    docker run -it -v %cd%/samples:/samples lang4iot/go bash
    docker run -it -v $(pwd)/../samples:/samples lang4iot/go bash

    tinygo build -o /samples/helloworld-go.wasm -target wasm /samples/helloworld-go.go
    