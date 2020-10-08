INSTALLATION :

tar -xvf *gz
./configure --enable-mpi --enable-double --prefix=/path/mary/NAME_OF_MY_INSTALLATION
(before export LDFLAGS=-L/path-of-my-fftw-installation/lib/, CPPFLAGS=-I/path-of-my-fftw-installation/include/)

make
make install-mdrun

RUN the code : mpirun -np NUMBER_OF_CORES /path/mary/NAME_OF_MY_INSTALLATION/bin/mdrun_d -v -s .tpr -deffnm name_of_my_files

TRPCAGE example file included with ./minput as separate input + tpr + structure/topology file (AMBER99SB)

For further information visit the website : www.gromacs.org
