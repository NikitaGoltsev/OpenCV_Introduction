# Introduction

Команды для запуска на gpu и cpu
test for cpu 
	pgcc file.c -pg -o file.out
	pgcc file.c -pg -ta=multicore -o file.out
	./file.out
	gprof file.out > text.txt

test for gpu
	pgcc file.c -acc -Minfo=accel -o file.out
	nvprof file.out


время: 
		 				float  				double

на cpu					0.07				0.08

на cpu/multicore		0.05				0.08 			

на gpu										0.0368

