# Singularity recipe file for fpocket

bootstrap: docker-daemon
from: fpocket/fpocket:001

%help
  First build the docker container:
    docker build -t fpocket/fpocket:001 .
  Then build this file:
    sudo singularity build fpocket.001.sif Singularity
  And run the rip script!
    singularity run --bind=`pwd`:/WORKDIR fpocket.001.sif -f /WORKDIR/data/sample/1UYD.pdb

%runscript
  fpocket "$@"
