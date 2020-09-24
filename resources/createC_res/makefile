SRC_DIR=src
OBJ_DIR=obj
BIN_DIR=bin

PROGRAM=prog

####### Compiler specifications #########@
COMPILER=gcc
CFLAGS=-Wall
GENPROG_FLAGS=-o

RULES=main.o

####### Source files ########

MAIN_SRC=$(SRC_DIR)/main.c

#############################

######## Dependecies ##########

MAIN_DEP= $(MAIN_SRC)

##############################

######### Object files ########

MAIN_OBJ=$(OBJ_DIR)/main.o

###############################

OBJECT_FILES=$(MAIN_OBJ) #the generated object files

all: $(RULES)
	$(COMPILER) $(OBJECT_FILES) $(GENPROG_FLAGS) $(BIN_DIR)/$(PROGRAM)

main.o: $(MAIN_DEP)
	$(COMPILER) $(MAIN_SRC) -c
	mv main.o $(MAIN_OBJ)