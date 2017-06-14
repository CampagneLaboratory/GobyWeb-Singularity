Bootstrap: docker
From: artifacts/base:latest 

%runscript

  echo "Nothing to do in this section"

%post
 
   echo "Here we are installing software and other dependencies for the container!"
   mkdir /gobyweb3
   cp ${HOME}/.bashrc /gobyweb3
   mkdir -p /scratchLocal/gobyweb
   mkdir -p /scratchLocal/gobyweb/FILESET_AREA
   mkdir -p /scratchLocal/gobyweb/JOB_AREA
   mkdir -p /scratchLocal/gobyweb/ARTIFACT_REPOSITORY
