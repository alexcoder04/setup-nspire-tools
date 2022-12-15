
# setup-nspire-tools

This is a GitHub Action that sets up all the tools needed for building TI-nspire Lua projects into `.tns` files.

## Tools installed

 - [Luna](https://github.com/ndless-nspire/Luna) as `luna` - building `.tns` files from Lua code
 - [nspire-merge](https://github.com/alexcoder04/nspire-merge) as `nspire-merge` - merging multiple Lua source files and images into one
 - [Sol](https://github.com/alexcoder04/sol-tools) as `sol` - building projects based on the [Sol framework](https://github.com/alexcoder04/sol-lib).

## Usage

```yml
name: ...

on:
  ...

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v3
    
    - name: Setup nspire Tools
      uses: alexcoder04/setup-nspire-tools@v1

    - name: ...
      run: ...

    ...
```
