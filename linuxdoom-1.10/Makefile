################################################################
#
# $Id:$
#
# $Log:$
#
CC=saturn-sh2-gcc

CFLAGS=-g
LDFLAGS=
LIBS=-lm

# subdirectory for objects
O=linux

SRCS= $(wildcard *.c)
OBJS= $(SRCS:.c=.o)

all:	 $(O)/linuxxdoom

clean:
	rm -f *.o *~ *.flc

$(O):
	mkdir $(O)

$(O)/linuxxdoom:	$(OBJS)
	$(CC) $(CFLAGS) $(LDFLAGS) $(OBJS) \
	-o $(O)/linuxxdoom $(LIBS)

$(O)/%.o:	%.c
	$(CC) $(CFLAGS) -c $< -o $@

#############################################################
#
#############################################################
