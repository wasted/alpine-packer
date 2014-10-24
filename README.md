brew install packer
packer build alpine-3.0.6.json
vagrant box add alpine64 build/alpine-3.0.6-amd64.box 

