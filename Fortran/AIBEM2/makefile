AIBEM2: AIBEM2.o AIBEM2_T.o GEOM2D.o H2LC.o CGLS.o FNHANK.o
	gfortran -L../gsl/lib -o AIBEM2 AIBEM2.o AIBEM2_T.o GEOM2D.o H2LC.o CGLS.o FNHANK.o -lfgsl -lgsl -lgslcblas

AIBEM2.o: AIBEM2.FOR
	gfortran -c AIBEM2.FOR

AIBEM2_T.o: AIBEM2_T.FOR
	gfortran -c AIBEM2_T.FOR

GEOM2D.o: ../SHARED/GEOM2D.FOR
	gfortran -c ../SHARED/GEOM2D.FOR

H2LC.o: ../SHARED/H2LC.FOR
	gfortran -c ../SHARED/H2LC.FOR

CGLS.o: ../SHARED/CGLS.FOR
	gfortran -c ../SHARED/CGLS.FOR

FNHANK.o: ../SHARED/FNHANK.FOR
	gfortran -I../gsl/include/fgsl -c ../SHARED/FNHANK.FOR

clean:
	rm AIBEM2.o AIBEM2_T.o GEOM2D.o H2LC.o CGLS.o FNHANK.o AIBEM2 AIBEM2.OUT
