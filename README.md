# GobyWeb-Singularity

Singularity repo to package docker artifacts:base:latest container for running GobyWeb plugins with Singularity

To build the image:

1. Install singularity (Mac: http://singularity.lbl.gov/install-mac) 
2. Activate the vagrant VM 
````
vagrant init singularityware/singularity-2.4
vagrant up
vagrant ssh
````
3. Inside the VM
````
cd /vagrant
git clone git@github.com:CampagneLaboratory/GobyWeb-Singularity.git
cd GobyWeb-Singularity/
sudo singularity build --writable CampagneLaboratory-GobyWeb-Singularity-master-latest.img shub://CampagneLaboratory/GobyWeb-Singularity
```` 
4. At this point, we can exit the VM and copy the image file: CampagneLaboratory-GobyWeb-Singularity-master-latest.img 
