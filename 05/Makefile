NAME		:= libft

CC			:= gcc

CFLAGS		:= -Wall -Wextra -Werror -g

SRCS_DIR	:= ./srcs

SRC			:= $(wildcard $(SRCS_DIR)/*.c)

OBJ			:= $(patsubst $(SRCS_DIR)/%.c, %.o, $(SRC))

INC			:= -Iinc

all			= $(NAME)

$(NAME)		: $(OBJ)
			$(CC) $(CFLAGS) $(OBJ) -o $@


%.o			: $(SRCS_DIR)/%.c
			$(CC) $(CFLAGS) $(INC) -c $< -o $@

clean		:
			$(RM) $(OBJ)

fclean		:
			$(RM) $(NAME)

re			: fclean all

.PHONY		: all clean fclean re






