NAME = zombie

CC = c++
CFLAGS = -Wall -Wextra -Werror

FILES = main.cpp	\
		newZombie.cpp	\
		randomChump.cpp	\
		Zombie.cpp		\

OFILES = ${FILES:%.cpp=%.o}

all: $(NAME)

$(NAME): $(OFILES)
	$(CC) $^ -o $@

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -rf $(OFILES)

fclean: clean
	rm -rf $(NAME)

re: fclean all

.PHONY: all clean fclean re
