# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: doreshev <doreshev@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/04/07 13:29:01 by doreshev          #+#    #+#              #
#    Updated: 2022/06/24 13:02:32 by doreshev         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = philo

CC = cc

RM = rm -f

FLAGS = -Wall -Wextra -Werror -g

SRC =	philo.c \
		philo_utils.c \
		ft_init.c \
		ft_thread.c \

OBJ = ${SRC:.c=.o}

.c.o:
	${CC} ${FLAGS} -c $< -o ${<:.c=.o}

${NAME}: ${OBJ}
		${CC} ${OBJ} -o ${NAME} 

all: ${NAME}

clean:
	${RM} ${OBJ}

fclean: clean
	${RM} ${NAME}

re: fclean all

.PHONY: all clean fclean re