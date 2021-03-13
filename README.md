# Libft

My personal C library.

Many recreated C Standard Library functions, & many additional functions used in further C projects ([Push_swap](https://github.com/dfinnis/Push_swap), [Lem_in](https://github.com/dfinnis/Lem_in), [Corewar](https://github.com/dfinnis/Corewar), & [md5](https://github.com/dfinnis/md5)).

At 42, using standard library functions (e.g. *atoi*) is forbidden, so students must create their own libft library from scratch.

#### Final Score 125/100


## Getting Started

First clone this repo.

```git clone https://github.com/dfinnis/Libft.git; cd Libft```

Make to compile *libft.a*.

```make```

Include *inc/libft.h* at the top of a C file, and compile with *libft.a*. Then you can use any of my libft functions.


### Example

At the root of this repo you'll find an example main *pseudo_cat.c*. *pseudo_cat.c* imports and uses my libft functions (*get_next_line* & *ft_printf* which use many other libft functions) to approximate the behaviour of *cat*.

Compile *pseudo_cat* with *libft.a* includes.

```gcc pseudo_cat.c libft.a -I includes -o pseudo_cat```

Run *pseudo_cat* with file as argument, just like *cat*.

```./pseudo_cat author; cat author```

<img src="https://github.com/dfinnis/Libft/blob/master/img/cat.png" width="470">


## Functions

See the [subject](https://github.com/dfinnis/Libft/blob/master/subject.pdf) for more details.

### Memory

* **bzero** - Write zeroed bytes to a string.
* **memalloc** - Allocate with malloc and return a “fresh” memory area.
* **memccpy** - Copy a string, until character *c*.
* **memchr** - Locate the first occurrence of a character in a string.
* **memcmp** - Compare strings.
* **memcpy** - Copy memory.
* **memdel** - Free memory.
* **memmove** - Copy a byte string.
* **memset** - Write len bytes of a value to a string.
* **calloc** - Allocate and zero memory.

### Convert number

* **atoi** - Ascii to int.
* **atoi_intmax** - Larger numbers.
* **itoa** - Int to ascii.
* **itoa_intmax** - Larger numbers.
* **itoa_unsigned** - Unsigned numbers.
* **itoa_base** - Specify base.
* **sqrt** - Square root.

### Put

* **putchar** - Write a character.
* **putchar_fd** - Write a character to file descriptor.
* **putendl** - Write a string to stdout followed by ’\n’.
* **putendl_fd** - Write a string to file descriptor followed by ’\n’.
* **putnbr** - Write an integer.
* **putnbr_fd** - Write an integer to file descriptor.
* **putstr** - Write a string.
* **putstr_fd** - Write a string to file descriptor.

### Character

* **isascii** - Is ascii.
* **isalpha** - Is alphabet.
* **isdigit** - Is number.
* **isalnum** - Is alphabet or number.
* **isprint** - Is printable.
* **isblank** - Is white space.
* **tolower** - Convert case to lower.
* **toupper** - Convert case to upper.
* **swap** - Swap characters.

### String

* **strcat** - Concatenate strings.
* **strchr** - Locate a character in string.
* **strclr** - Set every character of string to ’\0’.
* **strcmp** - Compare strings.
* **strcpy** - Copy a string.
* **strdel** - Free a string.
* **strdup** - Duplicate a string.
* **strequ** - Compare strings lexicographically. Return 1 if identical, 0 if different.
* **striter** - Apply function *f* to each character of a string.
* **striteri** - Apply function *f* to each character of a string by index.
* **strjoin** - Join strings.
* **strlcat** - Concatenate strings.
* **strlen** - Measure string length.
* **strmap** - Apply function *f* to each character of a malloced string.
* **strmapi** - Apply function *f* to each character of a malloced string by index.
* **strncat** - Concatenate strings until *n* bytes.
* **strncmp** - Compare *n* bytes of strings.
* **strncpy** - Copy *n* bytes a string.
* **strnequ** - Compare *n* bytes of strings lexicographically.
* **strnew** - Allocate fresh string.
* **strnstr** - Locate a substring in a string.
* **strrchr** - Locate a character in string.
* **strsplit** - Split a string using character *c* as delimiter, return as list.
* **strstr** - Locate a substring in a string.
* **strsub** - Create substring.
* **strtrim** - Trim whitespace.
* **strrev** - Reverse string.
* **strndup** - Duplicate *n* bytes of string.
* **strlcpy** - Copy a string.
* **split_whitespaces** - Split a string using whitespace as delimiter, return as list.

### Free

* **freestr** - Free a string.
* **strjoinfree** - Join strings, free original strings.
* **strjoinfree_s1** - Join strings, free string 1.
* **strjoinfree_s2** - Join strings, free string 2.
* **2d_int_free** - Free 2d int array.
* **2d_char_free** - Free 2d char array.

### List

* **lstnew** - New list element.
* **lstdelone** - Delete list element.
* **lstdel** - Delete entire list.
* **lstadd** - Add new element to the beginning of list.
* **lstiter** - Iterate list and apply function *f* to each element.
* **lstmap** - Iterate list and apply function *f* to each element, return new malloced list.
* **listlen_int** - Measure length of list of integers.
* **listlen_char** - Measure length of list of characters.

### Endianness

* **swap_endian** - Swap little <-> big endian, 32bit.
* **swap_endian64** - Swap little <-> big endian, 64bit.

### Further projects

* **get_next_line** - Read a file descriptor one line at a time.
* **ft_printf** - Printf() recoded.
* **ft_dprintf** - Print to file descriptor.


## Rigor

Like all 42 projects in C, this project must conform to the 42 Norm.
No leaks, errors handled carefully, & no unexpected quitting (seg fault, bus error, double free, etc.).
