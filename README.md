# Introduction

## Main Goal

This project ia an attempt to aggregate end to end toolchains for various programming languages to enable them on microcontrollers with special focus on ESP32 chips.

The idea is to provide examples, dockerfiles and instructions, so it shoudl be possible to follow simple process:

(1) Build an example for selected language to **wasm** file.

(2) Run compiled example on host machine

(3) Run compiled example on ESP32 simulator (QEMU) on host machine using using selected runtime

(4) Build and run example on ESP32 target using selected runtime


## Additional Goals

(1) Provide a template of using ESP IDF test framework with Linux and QEMU. 

(2) Study and define common API for IoT

(3) Performance comparison between various language implementations, WASM and non-WASM runtimes

(4) Swagger-like API definition

## Future Goals 

(1) Evolve into an underlying platform that can be used by maintainers of other platforms

# Languages

|             |Implementations                                                  |
|-------------|-----------------------------------------------------------------|
|C++          |[Emscripten](languages/c-cpp-via-emscripten/README.md)           |
|             |[Cheerp](languages/c-cpp-via-cheerp/README.md)                   |
|             |[Smooth](languages/c-cpp-via-smooth/c-cpp-smooth/README.md)      |
|             |[Native](languages/c-cpp-via-native/README.md)                   |
|C#           |[Blazor](languages/csharp-via-blazor/README.md)                  |
|             |[NanoFramework](languages/csharp-via-nanoframerwork)             |
|Go           |[TinyGo](languages/go)                                |
|Haskell      |[Haskell](languages/haskell)                                     |
|Java         |[Java](languages/java-via-teavm/README.md)                       |
|Kotlin       |[Kotlin](languages/kotlin-via-teavm/README.md)                   |
|Python       |[Python](languages/python-via-pyodide/README.md)                 |
|Rust         |[Rust](languages/rust/README.md)                                 |
|TypeScript   |[TypeScript](languages/typescript/README.md)  |
|Haxe         |[Haxe](languages/haxe/README.md)                                 |
|PHP          |[PHP](languages/php/README.md)                                   |
|Ruby         |[Ruby](languages/ruby/README.md)                                 |
|Swift        |[Swift](languages/swift/README.md)                               |

# Runtimes

|       |x86  |ESP32|
|-------|-----|-----|
|EOSVM  |     |     |
|Fizzy  |     |     |
|Wasm3  |     |     |
|wac    |     |     |
|wasmrt |     |     |
|wasmvm |     |     |
|WAVM   |     |     |
|WAMR   |     |     |


# API Bindings

Check details [here](api/api.md)


# Runtimes

## EOSVM

    https://github.com/EOSIO/eos-vm

## Fizzy

    https://github.com/wasmx/fizzy

## Wasm3

    https://github.com/wasm3/wasm3

    Tests running in QEMU
    https://github.com/wasm3/wasm3/blob/9dcfce271c2fac86823725fc9ec0f75309d820e4/.github/workflows/tests.yml#L491-L516

## wac

    https://github.com/kanaka/wac

## wasmrt

    https://github.com/rhitchcock/wasmrt

## wasmvm

    https://github.com/WasmVM/WasmVM

## WAVM

    https://github.com/WAVM/WAVM

## WAMR

    https://github.com/bytecodealliance/wasm-micro-runtime

# API Bindings

## WASI

TBD

## Custom ESP32

TBD

# Tools

## wabt

Suite of tools for WebAssembly:

    https://github.com/WebAssembly/wabt


# Simulation

## Renode

    https://renode.io

## Wokwi

    https://wokwi.com

## TinkerCAD

    https://www.tinkercad.com

