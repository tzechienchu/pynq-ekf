#
# Makefile for TinyEKF GPS example
#
# Copyright (C) 2015 Simon D. Levy
#
# MIT License

CC = gcc

SRC = .
OBJSH = gps_ekf.o tiny_ekf.o


all:
	$(CC) -fPIC -c -g3 gps_ekf.c
	$(CC) -fPIC -c -g3 tiny_ekf.c
	$(CC) -Wall -O3 -I. -I$(SRC) $(OBJSH) -o gps_ekf main.c -lm
	
run:
	./gps_ekf

clean:
	rm -f gps_ekf *.o *~ ekf.csv
