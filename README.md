# ft_printf

A custom implementation of the C standard library's `printf` function, developed as part of the 42 curriculum.

## Supported conversions

- `%c` — Character
- `%s` — String
- `%p` — Pointer address
- `%d` — Signed decimal integer
- `%i` — Signed integer
- `%u` — Unsigned decimal integer
- `%x` — Lowercase hexadecimal
- `%X` — Uppercase hexadecimal
- `%%` — Percent sign

The project builds the static library `libftprintf.a`.

## Build

```bash
make
```

## Make commands

```bash
make        # Build libftprintf.a
make clean  # Remove object files
make fclean # Remove object files and libftprintf.a
make re     # Rebuild everything
```

## Usage

```c
#include "ft_printf.h"
```

```bash
cc -Wall -Wextra -Werror main.c -L. -lftprintf -o program
```

Example:

```c
ft_printf("Hello, %s! Number: %d\\n", "42", 42);
```

## Source files

- `ft_printf.c` — Format parsing and dispatch
- `ft_str.c` — Character and string output
- `ft_int.c` — Integer and unsigned integer output
- `ft_hex.c` — Pointer and hexadecimal output

## Compiler flags

- `-Wall`
- `-Wextra`
- `-Werror`

## Author

**alperenocak**
