# C

## Data Types

Data Types define the allocated size of memory and the interpretation of the binary state.

The C data type `char` for example allocates the smallest unit of memory that can be addressed. On *allmost all* systems (64-bit and 32-bit CPU) the size of `char` has the size of a `byte` containing `8 bits`. `char` is used to represent characters in strings as well as intgers.

To give an understanding of how integer data types are represented in memory we introduce the integer data type `quat` consisting of `4 Bits` which in in memory looks as follows:

| Binary Representation | Decimal Number System (unsigned) | Decimal Number System (signed)
| ---------------------|---------|------|
| `0000` | `0` | `0`
| `0001` | `1` | `1`
| `0010` | `2` | `2`
| `0011` | `3` | `3` |
| `0100` | `4` | `4` |
| `0101` | `5` | `5` |
| `0110` | `6` | `6` |
| `0111` | `7` | `7` |
| `1000` | `8` | `-1` |
| `1001` | `9` | `-2` |
| `1010` | `10` | `-3` |
| `1011` | `11` | `-4` |
| `1100` | `12` | `-5`
| `1101` | `13` | `-6` |
| `1110` | `14` | `-7` |
| `1111` | `15` | `-8` |

### Top of the Primitive Datatypes

| Name | Memory Allocation | Used For |
|------|-------------------|----------|
| `char` | `1 Byte` | characters in strings and `signed/unsigned` integers. |
| `int` | `4 Bytes` | `signed/unsigned` integers. |
| `float` | `4 Bytes` | Single-Precision Floating Point/Decimal number. |
| `double` | `8 Bytes` | Double-Precision Floating Point/Decimal number. |

## Hello World

In order to write code you may choose your text editor of choice (like [Nano](https://www.nano-editor.org/), [Sublime](https://www.sublimetext.com/), [Atom](https://atom.io/), [VS Code](https://code.visualstudio.com/) or hardcore terminal UX with [Emacs](https://www.gnu.org/software/emacs/)) and create a new file called `main.c`. The following code will print "Hello World" when the compiled binary is executed:

```
#include <stdio.h>

int main(void)
{
    printf("Hello World\n");

    return 0;
}
```

## Setup & Compilation

You can [compile](https://en.wikipedia.org/wiki/Compiler) your application in a terminal by providing your file (`main.c`) to a C compiler. By using a flag (`-o`) you can specify the name of the binary the compiler produces:

```
$ cc main.c -o first.app
```

Then execute the binary:

```
$ ./first.app
```

You can find good summaries and information concerning terminal navigation/applications in the [web](http://www.informit.com/blogs/blog.aspx?uk=The-10-Most-Important-Linux-Commands).
