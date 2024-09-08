
SRC = ft_putchar.c ft_putstr.c ft_strcmp.c ft_strlen.c ft_swap.c
PRE = ./sources/
NAME = libft.a
SRCS = ${addprefix ${PRE}, ${SRC}}
OBJS = ${SRCS:.c=.o}
INCLUDES = ./includes/
CFLAGS += -Wall -Wextra -Werror -I includes

all: ${NAME}
.c.o:
	cc ${CFLAGS} -c -I${INCLUDES} $< -o ${<:.c=.o}
${NAME}: ${OBJS}
			ar rcs ${NAME} ${OBJS}
			ranlib ${NAME}
clean:
	rm -f ${OBJS}
fclean:
	rm -f ${NAME}
re:
	fclean all
.PHONY: all clean fclean re
