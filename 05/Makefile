NAME				:= libft

CC					:= gcc

CFLAGS				:= -Wall -Wextra -Werror -g

SRCS_DIR			:= ./srcs

SRC					:= $(wildcard $(SRCS_DIR)/*.c)

OBJ					:= $(patsubst $(SRCS_DIR)/%.c, $(SRCS_DIR)/%.o, $(SRC))

INC					:= -Iinc

all					: $(NAME)

$(NAME)				: $(OBJ)
						$(CC) $(CFLAGS) $(OBJ) -o $@

$(SRCS_DIR)/%.o		: $(SRCS_DIR)/%.c
						$(CC) $(CFLAGS) $(INC) -c $< -o $@

clean				:
						$(RM) $(OBJ)

fclean				: clean
						$(RM) $(NAME)

re					: fclean all

.PHONY				: all clean fclean re






