<div align="center">
  <h1>Pybfc</h1>
  <p>Pybfc - BranFuck compiler write in python</p>
  <a href="https://pypi.org/project/pybfc/">
    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/pybfc?color=9cf">
  </a>
  <a href="https://pypi.org/project/pybfc/">
    <img alt="PyPI" src="https://img.shields.io/pypi/v/pybfc?color=9cf">
  </a>
  <a href="https://www.gnu.org/licenses/agpl-3.0.en.html">
    <img src="https://img.shields.io/pypi/l/pybfc?color=9cf&label=License" alt="License">
  </a>
  <br>
  <a href="https://github.com/TheAwiteb/pybfc/actions/workflows/python-app.yml">
    <img alt="test-pybfc" src="https://github.com/TheAwiteb/pybfc/actions/workflows/python-app.yml/badge.svg">
  </a>
  <a href="https://github.com/TheAwiteb/pybfc/actions/workflows/release.yml">
    <img alt="Upload Python Package" src="https://github.com/TheAwiteb/pybfc/actions/workflows/release.yml/badge.svg">
  </a>
  <br>
  <a href="https://github.com/psf/black">
    <img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
  </a>
</div>
  
<details open>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#Requirements">Requirements</a>
    </li>
    <li>
      <a href="#Installation">Installation</a>
      <ul>
        <li><a href="#PyPi">With PyPi</a></li>
        <li><a href="#GitHub">With GitHub</a></li>
      </ul>
    </li>
    <li><a href="#Usage">Usage</a></li>
    <li>
      <a href="#Examples">Examples</a>
        <ul>
            <li><a href="#Debug">Debug</a></li>
            <li><a href="#Hello-World">Hello World</a></li>
        </ul>
    </li>
    <li><a href="#Discussions">Discussions</a></li>
    <li><a href="#Issues">Issues</a></li>
    <li><a href="#Donating">Donating</a></li>
    <li><a href="#License">License</a></li>
  </ol>
</details>


## Requirements

* [Python](https://Python.org/) >= 3.8

## Installation

### PyPi

```bash
$ pip3 install pybfc
```

### GitHub

```bash
$ git clone https://github.com/TheAwiteb/pybfc
$ cd pybfc
$ python3 setup.py install
```

## Usage
```
Usage: pybfc [OPTIONS] FILE_PATH

  Python BranFuck Compiler ???????

Arguments:
  FILE_PATH  BranFuck path to execute it.  [required]

Options:
  -d, --debug    Enable debugging with execution.
  -V, --version  Print Pybfc version and exit.
  --help         Show this message and exit.
```

## Examples
### Debug
```main.bf```
```BranFuck
>++<
```
```bash
?? pybfc --debug main.bf
Command -> '>', Loop -> 0
        Address -> 1, Value -> 0

Command -> '+', Loop -> 0
        Address -> 1, Value -> 1

Command -> '+', Loop -> 0
        Address -> 1, Value -> 2

Command -> '<', Loop -> 0
        Address -> 0, Value -> 0
```

### Hello World
```main.bf```
```BranFuck
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.
>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
```
```bash
?? pybfc main.bf
Hello World!

```

## Discussions
Question, feature request, discuss about pybfc [here](https://github.com/TheAwiteb/pybfc/discussions)

## Issues
You can report a bug from [here](https://github.com/TheAwiteb/pybfc/issues/new?assignees=&labels=bug&template=bug.md)


## Donating
> Note: These addresses are for BEP20 tokens

|    Currency          |                Address                          |
| ---------------------|------------------------------------------------ |
| Binance **BNB**| ```0x4ab0974c7dfcdcdf24d8323a93b061d41e9cf3f0```|
| Binance USD **BUSD**  | ```0x4ab0974c7dfcdcdf24d8323a93b061d41e9cf3f0```|
| Tether **USDT** | ```0x4ab0974c7dfcdcdf24d8323a93b061d41e9cf3f0``` |
| Bitcoin **BTC**  | ```0x4ab0974c7dfcdcdf24d8323a93b061d41e9cf3f0```|
| Bitcoin Cash **BCH**| ```0x4ab0974c7dfcdcdf24d8323a93b061d41e9cf3f0```|

## License

[GNU Affero General Public Version 3](https://www.gnu.org/licenses/agpl-3.0.en.html) License
