# Singularity recipe file for fpocket

bootstrap: docker-daemon
from: fpocket/fpocket:004

%help
  First build the docker container:
    docker build -t fpocket/fpocket:004 .
  Then build this file:
    sudo singularity build fpocket.004.sif Singularity
  And run the rip script!
    singularity run --bind=`pwd`:/WORKDIR fpocket.004.sif -f /WORKDIR/data/sample/1UYD.pdb

%runscript
  fpocket "$@"
