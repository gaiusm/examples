CCFLAGS = -I. -g

all: force
	g++ $(CCFLAGS) -O0 fib.cc
	valgrind ./a.out
	g++ $(CCFLAGS) -O3 fibspeed.cc
	valgrind ./a.out
	time ./a.out
	g++ $(CCFLAGS) -O3 fibiter.cc
	valgrind ./a.out
	time ./a.out

clean: force
	$(RM) *.o a.out *~

force:
