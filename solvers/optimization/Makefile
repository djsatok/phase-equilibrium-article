CXX=g++
CXXFLAGS= -O3 -g

LIBS=

all: main

%.o: %.cpp
	$(CXX) -c -o $@ $< $(CXXFLAGS)

main: main.o PhaseSolver.o
	$(CXX) $(LDFLAGS) -o $@ $^ $(LIBS)

clean:
	rm -f *.o main *~ out.csv
