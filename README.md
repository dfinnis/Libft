# Libft

My personal C library.

Many recreated C Standard Library functions, & many additional functions used in further C projects ([Push_swap](https://github.com/dfinnis/Push_swap), [Lem_in](https://github.com/dfinnis/Lem_in), [Corewar](https://github.com/dfinnis/Corewar), & [md5](https://github.com/dfinnis/md5)).

At 42, using standard library functions (e.g. *atoi*) is forbidden, so students must create their own libft library from scratch.

*Final Score 125/100*


## Getting Started

First clone this repo. <br>
```git clone https://github.com/dfinnis/Libft.git; cd Libft```

Make to compile *libft.a*. <br>
```make```

Include *inc/libft.h* at the top of a C file, and compile with *libft.a*. Then you can use any of my libft functions.


### Example

At the root of this repo you'll find an example main *pseudo_cat.c*. *pseudo_cat.c* uses my libft functions (*get_next_line* & *ft_printf* which use many other libft functions) to approximate the behaviour of *cat*.

Compile *pseudo_cat* with *libft.a* includes. <br>
```gcc pseudo_cat.c libft.a -I includes -o pseudo_cat```

Run *pseudo_cat* with file as argument, just like *cat*. <br>
```./pseudo_cat author; cat author```

<img src="https://github.com/dfinnis/Libft/blob/master/img/cat.png" width="470">


## Functions

See the [subject](https://github.com/dfinnis/Libft/blob/master/subject.pdf) for more details.

### Memory

* [**bzero**](https://github.com/dfinnis/Libft/blob/master/src/ft_bzero.c) - Write zeroed bytes to a string.
* [**memalloc**](https://github.com/dfinnis/Libft/blob/master/src/ft_memalloc.c) - Allocate with malloc and return a “fresh” memory area.
* [**memccpy**](https://github.com/dfinnis/Libft/blob/master/src/ft_memccpy.c) - Copy a string, until character *c*.
* [**memchr**](https://github.com/dfinnis/Libft/blob/master/src/ft_memchr.c) - Locate the first occurrence of a character in a string.
* [**memcmp**](https://github.com/dfinnis/Libft/blob/master/src/ft_memcmp.c) - Compare strings.
* [**memcpy**](https://github.com/dfinnis/Libft/blob/master/src/ft_memcpy.c) - Copy memory.
* [**memdel**](https://github.com/dfinnis/Libft/blob/master/src/ft_memdel.c) - Free memory.
* [**memmove**](https://github.com/dfinnis/Libft/blob/master/src/ft_memmove.c) - Copy a byte string.
* [**memset**](https://github.com/dfinnis/Libft/blob/master/src/ft_memset.c) - Write len bytes of a value to a string.
* [**calloc**](https://github.com/dfinnis/Libft/blob/master/src/ft_calloc.c) - Allocate and zero memory.

### Convert number

* [**atoi**](https://github.com/dfinnis/Libft/blob/master/src/ft_atoi.c) - Ascii to int.
* [**atoi_intmax**](https://github.com/dfinnis/Libft/blob/master/src/ft_atoi_intmax.c) - Larger numbers.
* [**itoa**](https://github.com/dfinnis/Libft/blob/master/src/ft_itoa.c) - Int to ascii.
* [**itoa_intmax**](https://github.com/dfinnis/Libft/blob/master/src/ft_itoa_intmax.c) - Larger numbers.
* [**itoa_unsigned**](https://github.com/dfinnis/Libft/blob/master/src/ft_itoa_unsigned.c) - Unsigned numbers.
* [**itoa_base**](https://github.com/dfinnis/Libft/blob/master/src/ft_itoa_base.c) - Specify base.
* [**sqrt**](https://github.com/dfinnis/Libft/blob/master/src/ft_sqrt.c) - Square root.

### Put

* [**putchar**](https://github.com/dfinnis/Libft/blob/master/src/ft_putchar.c) - Write a character.
* [**putchar_fd**](https://github.com/dfinnis/Libft/blob/master/src/ft_putchar_fd.c) - Write a character to file descriptor.
* [**putendl**](https://github.com/dfinnis/Libft/blob/master/src/ft_putendl.c) - Write a string to stdout followed by ’\n’.
* [**putendl_fd**](https://github.com/dfinnis/Libft/blob/master/src/ft_putendl_fd.c) - Write a string to file descriptor followed by ’\n’.
* [**putnbr**](https://github.com/dfinnis/Libft/blob/master/src/ft_putnbr.c) - Write an integer.
* [**putnbr_fd**](https://github.com/dfinnis/Libft/blob/master/src/ft_putnbr_fd.c) - Write an integer to file descriptor.
* [**putstr**](https://github.com/dfinnis/Libft/blob/master/src/ft_putstr.c) - Write a string.
* [**putstr_fd**](https://github.com/dfinnis/Libft/blob/master/src/ft_putstr_fd.c) - Write a string to file descriptor.

### Character

* [**isascii**](https://github.com/dfinnis/Libft/blob/master/src/ft_isascii.c) - Is ascii.
* [**isalpha**](https://github.com/dfinnis/Libft/blob/master/src/ft_isalpha.c) - Is alphabet.
* [**isdigit**](https://github.com/dfinnis/Libft/blob/master/src/ft_isdigit.c) - Is number.
* [**isalnum**](https://github.com/dfinnis/Libft/blob/master/src/ft_isalnum.c) - Is alphabet or number.
* [**isprint**](https://github.com/dfinnis/Libft/blob/master/src/ft_isprint.c) - Is printable.
* [**isblank**](https://github.com/dfinnis/Libft/blob/master/src/ft_isblank.c) - Is white space.
* [**tolower**](https://github.com/dfinnis/Libft/blob/master/src/ft_tolower.c) - Convert case to lower.
* [**toupper**](https://github.com/dfinnis/Libft/blob/master/src/ft_toupper.c) - Convert case to upper.
* [**swap**](https://github.com/dfinnis/Libft/blob/master/src/ft_swap.c) - Swap characters.

### String

* [**strcat**](https://github.com/dfinnis/Libft/blob/master/src/ft_strcat.c) - Concatenate strings.
* [**strchr**](https://github.com/dfinnis/Libft/blob/master/src/ft_strchr.c) - Locate a character in string.
* [**strclr**](https://github.com/dfinnis/Libft/blob/master/src/ft_strclr.c) - Set every character of string to ’\0’.
* [**strcmp**](https://github.com/dfinnis/Libft/blob/master/src/ft_strcmp.c) - Compare strings.
* [**strcpy**](https://github.com/dfinnis/Libft/blob/master/src/ft_strcpy.c) - Copy a string.
* [**strdel**](https://github.com/dfinnis/Libft/blob/master/src/ft_strdel.c) - Free a string.
* [**strdup**](https://github.com/dfinnis/Libft/blob/master/src/ft_strdup.c) - Duplicate a string.
* [**strequ**](https://github.com/dfinnis/Libft/blob/master/src/ft_strequ.c) - Compare strings lexicographically. Return 1 if identical, 0 if different.
* [**striter**](https://github.com/dfinnis/Libft/blob/master/src/ft_striter.c) - Apply function *f* to each character of a string.
* [**striteri**](https://github.com/dfinnis/Libft/blob/master/src/ft_striteri.c) - Apply function *f* to each character of a string by index.
* [**strjoin**](https://github.com/dfinnis/Libft/blob/master/src/ft_strjoin.c) - Join strings.
* [**strlcat**](https://github.com/dfinnis/Libft/blob/master/src/ft_strlcat.c) - Concatenate strings.
* [**strlen**](https://github.com/dfinnis/Libft/blob/master/src/ft_strlen.c) - Measure string length.
* [**strmap**](https://github.com/dfinnis/Libft/blob/master/src/ft_strmap.c) - Apply function *f* to each character of a malloced string.
* [**strmapi**](https://github.com/dfinnis/Libft/blob/master/src/ft_strmapi.c) - Apply function *f* to each character of a malloced string by index.
* [**strncat**](https://github.com/dfinnis/Libft/blob/master/src/ft_strncat.c) - Concatenate strings until *n* bytes.
* [**strncmp**](https://github.com/dfinnis/Libft/blob/master/src/ft_strncmp.c) - Compare *n* bytes of strings.
* [**strncpy**](https://github.com/dfinnis/Libft/blob/master/src/ft_strncpy.c) - Copy *n* bytes a string.
* [**strnequ**](https://github.com/dfinnis/Libft/blob/master/src/ft_strnequ.c) - Compare *n* bytes of strings lexicographically.
* [**strnew**](https://github.com/dfinnis/Libft/blob/master/src/ft_strnew.c) - Allocate fresh string.
* [**strnstr**](https://github.com/dfinnis/Libft/blob/master/src/ft_strnstr.c) - Locate a substring in a string.
* [**strrchr**](https://github.com/dfinnis/Libft/blob/master/src/ft_strrchr.c) - Locate a character in string.
* [**strsplit**](https://github.com/dfinnis/Libft/blob/master/src/ft_strsplit.c) - Split a string using character *c* as delimiter, return as list.
* [**strstr**](https://github.com/dfinnis/Libft/blob/master/src/ft_strstr.c) - Locate a substring in a string.
* [**strsub**](https://github.com/dfinnis/Libft/blob/master/src/ft_strsub.c) - Create substring.
* [**strtrim**](https://github.com/dfinnis/Libft/blob/master/src/ft_strtrim.c) - Trim whitespace.
* [**strrev**](https://github.com/dfinnis/Libft/blob/master/src/ft_strrev.c) - Reverse string.
* [**strndup**](https://github.com/dfinnis/Libft/blob/master/src/ft_strndup.c) - Duplicate *n* bytes of string.
* [**strlcpy**](https://github.com/dfinnis/Libft/blob/master/src/ft_strlcpy.c) - Copy a string.
* [**split_whitespaces**](https://github.com/dfinnis/Libft/blob/master/src/ft_split_whitespaces.c) - Split a string using whitespace as delimiter, return as list.

### Free

* [**freestr**](https://github.com/dfinnis/Libft/blob/master/src/ft_freestr.c) - Free a string.
* [**strjoinfree**](https://github.com/dfinnis/Libft/blob/master/src/ft_strjoinfree.c) - Join strings, free original strings.
* [**strjoinfree_s1**](https://github.com/dfinnis/Libft/blob/master/src/ft_strjoinfree_s1.c) - Join strings, free string 1.
* [**strjoinfree_s2**](https://github.com/dfinnis/Libft/blob/master/src/ft_strjoinfree_s2.c) - Join strings, free string 2.
* [**2d_int_free**](https://github.com/dfinnis/Libft/blob/master/src/ft_2d_int_free.c) - Free 2d int array.
* [**2d_char_free**](https://github.com/dfinnis/Libft/blob/master/src/ft_2d_char_free.c) - Free 2d char array.

### List

* [**lstnew**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstnew.c) - New list element.
* [**lstdelone**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstdelone.c) - Delete list element.
* [**lstdel**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstdel.c) - Delete entire list.
* [**lstadd**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstadd.c) - Add new element to the beginning of list.
* [**lstiter**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstiter.c) - Iterate list and apply function *f* to each element.
* [**lstmap**](https://github.com/dfinnis/Libft/blob/master/src/ft_lstmap.c) - Iterate list and apply function *f* to each element, return new malloced list.
* [**listlen_int**](https://github.com/dfinnis/Libft/blob/master/src/ft_listlen_int.c) - Measure length of list of integers.
* [**listlen_char**](https://github.com/dfinnis/Libft/blob/master/src/ft_listlen_char.c) - Measure length of list of characters.

### Endianness

* [**swap_endian**](https://github.com/dfinnis/Libft/blob/master/src/swap_endian.c) - Swap little <-> big endian, 32bit.
* [**swap_endian64**](https://github.com/dfinnis/Libft/blob/master/src/swap_endian.c) - Swap little <-> big endian, 64bit.

### Further projects

* [**get_next_line**](https://github.com/dfinnis/Libft/blob/master/src/get_next_line.c) - Read a file descriptor one line at a time.
* [**ft_printf**](https://github.com/dfinnis/Libft/tree/master/src/ft_printf) - Printf() recoded.
* [**ft_dprintf**](https://github.com/dfinnis/Libft/blob/master/src/ft_printf/ft_dprintf.c) - Print to file descriptor.


## Rigor

Like all 42 projects in C, this project must conform to the 42 Norm.
No leaks, errors handled carefully, & no unexpected quitting (seg fault, bus error, double free, etc.).
