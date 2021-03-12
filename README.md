# Libft

My personal C library.

Many recreated C Standard Library functions.

Many additional functions used in further C projects ([Push_swap](https://github.com/dfinnis/Push_swap), [Lem_in](https://github.com/dfinnis/Lem_in), [Corewar](https://github.com/dfinnis/Corewar), & [md5](https://github.com/dfinnis/md5))

At 42, using standard library functions (e.g. *atoi*) is forbidden, so students must create their own libft library from scratch.

#### Final Score 125/100


## Getting Started

First clone this repo.

```git clone https://github.com/dfinnis/Libft.git; cd Libft```

Make to compile.

```make; make clean```

Include *ft_printf/ft_printf.h* at the top of a C file, then you can use any of the libft functions.

### Example

Let's create an example *pseudo_cat.c* at the root of this project.

```c
#include "ft_printf/ft_printf.h"
#include <fcntl.h>

int main (int ac, char **av)
{
    char *str;
    int fd;

    fd = open(av[1], O_RDONLY);
    while (get_next_line(fd, &str) == 1)
    {
        ft_printf("%s\n", str);
        free(str);
    }
    free(str);
    close (fd);
    return (0);
}
```

Compile *pseudo_cat* with ft_printf/libftprintf.a includes.

```gcc pseudo_cat.c ft_printf/libftprintf.a -I includes -o pseudo_cat```

*pseudo_cat* behaves similarly to *cat*.

<img src="https://github.com/dfinnis/Libft/blob/master/img/cat.png" width="40%">


## Functions

See the [subject](https://github.com/dfinnis/Libft/blob/master/subject.pdf) for more details.

### Memory

* **bzero** - 
* **memalloc** - 
* **memccpy** - 
* **memchr** - 
* **memcmp** - 
* **memcpy** - 
* **memdel** - 
* **memmove** - 
* **memset** - 
* **calloc** - 

### Convert number

* **atoi** - 
* **atoi_intmax** - 
* **itoa** - 
* **itoa_intmax** - 
* **itoa_unsigned** - 
* **itoa_base** - 
* **sqrt** - 

### Put

* **putchar** - 
* **putchar_fd** - 
* **putendl** - 
* **putendl_fd** - 
* **putnbr** - 
* **putnbr_fd** - 
* **putstr** - 
* **putstr_fd** - 

### Character is

* **isascii** - 
* **isalpha** - 
* **isdigit** - 
* **isalnum** - 
* **isprint** - 
* **isblank** - 

### String

* **strcat** - 
* **strchr** - 
* **strclr** - 
* **strcmp** - 
* **strcpy** - 
* **strdel** - 
* **strdup** - 
* **strequ** - 
* **striter** - 
* **striteri** - 
* **strjoin** - 
* **strlcat** - 
* **strlen** - 
* **strmap** - 
* **strmapi** - 
* **strncat** - 
* **strncmp** - 
* **strncpy** - 
* **strnequ** - 
* **strnew** - 
* **strnstr** - 
* **strrchr** - 
* **strsplit** - 
* **strstr** - 
* **strsub** - 
* **strtrim** - 
* **strrev** - 
* **strndup** - 
* **strlcpy** - 
* **tolower** - 
* **toupper** - 
* **split_whitespaces** - 

### Free

* **freestr** - 
* **strjoinfree** - 
* **strjoinfree_s1** - 
* **strjoinfree_s2** - 
* **2d_int_free** - 
* **2d_char_free** - 

### List

* **lstnew** - 
* **lstdelone** - 
* **lstdel** - 
* **lstadd** - 
* **lstiter** - 
* **lstmap** - 
* **listlen_int** - 
* **listlen_char** - 

### Swap

* **swap** - 
* **swap_endian** - 
* **swap_endian64** - 

### Further projects

* **get_next_line** - 
* **ft_printf** - 
* **ft_dprintf** - 


## Rigor

Like all 42 projects in C, this project must conform to the 42 Norm.
No leaks, errors handled carefully, & no unexpected quitting (seg fault, bus error, double free, etc.).
