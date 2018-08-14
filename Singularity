BootStrap: docker
From: debian:9
 
%label
    Maintainer remi-andre.olsen@scilifelab.se

%post
    apt-get update
    apt-get install -y git build-essential cmake libomp-dev zlib1g-dev 

    cd /opt
    git clone https://github.com/gonzalogacc/w2rap-contigger.git
    cd w2rap-contigger
    cmake -D CMAKE_CXX_COMPILER=g++ .  
    make -j 4
    make install
    
