include ../../Makefile.in
include ../../ParOpt_Common.mk

default: sellar.o
	${CXX} ${CCFLAGS} -o sellar sellar.o ${PAROPT_LD_FLAGS}

debug: CCFLAGS=${CCFLAGS_DEBUG}
debug: default

complex: CCFLAGS+=-DPAROPT_USE_COMPLEX
complex: default

clean:
	${RM} sellar *.o
