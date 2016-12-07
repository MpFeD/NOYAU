CC=gcc -Wall -ansi
BIN=bin
INC=include
LIB=lib
OBJ=obj
SRC=src




all: directories ${BIN}/noyau-tp1


directories: ${OBJ} ${BIN} ${LIB} ${SRC} ${INC}

${OBJ}:
	mkdir ${OBJ}
${BIN}:
	mkdir ${BIN}
${LIB}:
	mkdir ${LIB}
${SRC}:
	mkdir ${SRC}
${INC}:
	mkdir ${INC}



${BIN}/noyau-tp1: ${OBJ}/noyau-tp1.o
	gcc -o ${BIN}/noyau-tp1 ${OBJ}/noyau-tp1.o

${OBJ}/noyau-tp1.o: ${SRC}/noyau-tp1.c
	gcc -o ${OBJ}/noyau-tp1.o -c ${SRC}/noyau-tp1.c



clean:
	rm -rf ${OBJ} ${BIN} ${LIB}
	rm -f ${INC}/*~ ${SRC}/*~ *~
