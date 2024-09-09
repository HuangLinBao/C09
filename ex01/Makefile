
SRC = ft_putchar.c ft_putstr.c ft_strcmp.c ft_strlen.c ft_swap.c
PRE = ./srcs/
NAME = libft.a
SRCS = ${addprefix ${PRE}, ${SRC}}
OBJS = ${SRCS:.c=.o}
INCLUDES = ./includes/
CFLAGS += -Wall -Wextra -Werror -I includes

all: ${NAME}
.c.o:
	$(CC) $(CFLAGS) -c $< -o $@

$(NAME): $(OBJS)
	ar rcs $(NAME) $(OBJS)
clean:
	rm -f ${OBJS}
fclean: clean
	rm -f $(NAME)
re: fclean all
.PHONY: all clean fclean re