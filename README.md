# ft_printf

**ft_printf** is a project from the **School 42 curriculum** that challenges you to recreate the behavior of the standard C function `printf()`.  

It reinforces your understanding of:
- **Variadic functions** (`stdarg.h`)
- **String and number formatting**
- **Memory and buffer management**
- **Low-level output handling**

You will write a custom version of `printf` that behaves identically to the original for the allowed conversions.

---

## Features

### 1. **Supported Conversions**
Your `ft_printf` must handle the following format specifiers:

| Specifier | Description | Example |
|------------|--------------|----------|
| `%c` | Print a single character | `'A' → A` |
| `%s` | Print a string | `"Hello" → Hello` |
| `%p` | Print a pointer address | `0x7ffeea1f42c0` |
| `%d` | Print a signed decimal integer | `42 → 42` |
| `%i` | Print a signed integer (same as `%d`) | `-42 → -42` |
| `%u` | Print an unsigned decimal integer | `3000000000 → 3000000000` |
| `%x` | Print a number in lowercase hexadecimal | `255 → ff` |
| `%X` | Print a number in uppercase hexadecimal | `255 → FF` |
| `%%` | Print a literal `%` character | `% → %` |

---

### 2. **Core Functions**
You must implement the following:

| Function | Description |
|-----------|--------------|
| `ft_printf()` | Main function that parses the format string and prints arguments |
| `ft_putchar_fd()` | Print a single character |
| `ft_putstr_fd()` | Print a string |
| `ft_putnbr_fd()` | Print an integer |
| `ft_puthex_fd()` | Print numbers in hexadecimal |
| `ft_putptr_fd()` | Print a pointer address |
| Helper functions | For counting length, managing base conversions, etc. |

---

### 3. **Variadic Function Handling**
Use the C standard header `<stdarg.h>` for handling variable argument lists:
```c
#include <stdarg.h>

int ft_printf(const char *format, ...)
{
    va_list args;
    va_start(args, format);
    // handle each argument depending on format
    va_end(args);
    return (printed_chars);
}
