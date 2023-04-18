sandbox: libkk5k.so sandbox.o
	$(CXX) -o sandbox  sandbox.o -L. -lkk5k

libkk5k.so: kk5k.cpp
	$(CXX) -fPIC -c kk5k.cpp -o kk5k.o
	$(CXX) -shared -Wl,-soname,libkk5k.so -o libkk5k.so kk5k.o

clean:
	${RM} *.o *.so sandbox
