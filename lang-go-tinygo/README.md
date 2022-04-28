# TinyGo

## Example

    docker run -it -v %cd%/samples:/samples zimkal/wasm-go bash

    tinygo build -o /samples/helloworld-go.wasm -target wasm /samples/helloworld-go.go
    