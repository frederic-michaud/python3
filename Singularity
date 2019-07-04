Bootstrap: docker
From: ubuntu 

%help



%environment
  # use bash as default shell
  SHELL=/bin/bash
  export SHELL

%setup
  # runs on host - the path to the image is $SINGULARITY_ROOTFS

%post

  apt-get update
  apt-get install -y python3 python3-pip git
  apt-get clean
  pip3 install numpy matplotlib sklearn 
  pip3 install scikit-bio
  pip3 install astropy
  pip3 install numpy
%runscript
  # executes with the singularity run command
  # delete this section to use existing docker ENTRYPOINT command
