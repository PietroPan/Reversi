# source files.

SRC = menu.c bot.c load_save.c print_functions.c valid.c stack.c menu_options.c jogar.c main.c

OBJ = $(SRC:.cpp=.o)

OUT = reversi

# include directories
INCLUDES = -I.

# compiler
CCC = gcc 

.SUFFIXES: .cpp .c 

default: $(OUT)

.cpp.o:
	$(CCC) $(CCFLAGS) $(INCLUDES)  -c $< -o $@

.c.o:
	$(CCC) $(CCFLAGS) $(INCLUDES) -c $< -o $@

$(OUT): $(OBJ)
	$(CCC) -o $(OUT) $(CCFLAGS) $(OBJ) $(LIBS) 

clean:
	rm -f *.o .a *~ Makefile.bak $(OUT)

