CMAKE_FLAGS=""

ifdef RELEASE
    CMAKE_FLAGS+=-DCMAKE_BUILD_TYPE=Release
else
    CMAKE_FLAGS+=-DCMAKE_BUILD_TYPE=Debug
endif

top-master: all

check: all
	cd build && ctest

clean:
	${RM} -r build

.DEFAULT:
	mkdir -p build
	${LOAD_ENV}; cd build && cmake .. ${CMAKE_FLAGS} && ${MAKE} $@


