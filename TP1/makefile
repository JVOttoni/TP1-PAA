CC = gcc
CFLAGS = -Wall -g

# Incluir FilaPri.o na lista de objetos
OBJ = main.o grafo.o dijkstra.o uteis.o FilaPri.o

programa: $(OBJ)
	$(CC) $(CFLAGS) -o programa $(OBJ)

main.o: main.c prototipo.h
	$(CC) $(CFLAGS) -c main.c

grafo.o: grafo.c prototipo.h
	$(CC) $(CFLAGS) -c grafo.c

dijkstra.o: dijkstra.c prototipo.h
	$(CC) $(CFLAGS) -c dijkstra.c

uteis.o: uteis.c prototipo.h
	$(CC) $(CFLAGS) -c uteis.c

# Adicionando uma regra para compilar FilaPri.o
FilaPri.o: FilaPri.c prototipo.h
	$(CC) $(CFLAGS) -c FilaPri.c

clean:
	rm -f *.o programa

.PHONY: clean
