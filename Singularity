Bootstrap: docker
From: artifacts/base:1.5.4

%runscript

  echo "Nothing to do in this section"

%post
 
   echo "Here we are installing software and other dependencies for the container!"
   mkdir /gobyweb3
   cp ${HOME}/.bashrc /gobyweb3
   mkdir -p /scratchLocal/gobyweb
   mkdir -p /scratchLocal/gobyweb/gobyweb3
   mkdir -p /scratchLocal/gobyweb/gobyweb3/ARTIFACT_REPOSITORY-PLUGINS-SDK
   mkdir -p /scratchLocal/gobyweb/gobyweb3/FILESET_AREA
   mkdir -p /scratchLocal/gobyweb/gobyweb3/GOBYWEB_SGE_JOBS
   mkdir -p /scratchLocal/gobyweb/FILESET_AREA
   mkdir -p /scratchLocal/gobyweb/JOB_AREA
   mkdir -p /scratchLocal/gobyweb/ARTIFACT_REPOSITORY
   rm -fr /etc/mail
   mkdir -p /etc/mail

%test

  if [ ! -d /scratchLocal/gobyweb ]; then
	echo "%post did not run"
	exit 127
  fi
