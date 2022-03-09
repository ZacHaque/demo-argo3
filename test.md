

**WSL**

1. asdas
2. asdasda


**Proxy**

1. set up cntlm - downloaed .deb file from s3, install with dpkg
2. configure cntlm on secondary port like 3129
3. set evronment to point to proxy `https_proxy=http://127.0.0.1:3129`
4. started `cntlm`
5. put export command on the `~/.bashrc`

**apt inatall**

1. Import cert from s3 and install as suggested [here](https://ubuntu.com/server/docs/security-trust-store) 
2. Set proxy exclusively for apt to work, [link](https://www.serverlab.ca/tutorials/linux/administration-linux/how-to-set-the-proxy-for-apt-for-ubuntu-18-04/)
3. install required apt packages including pip

**pip3**

1. If faces ssl issues installing `pip3 install aws-mfa` check [here](https://pip.pypa.io/en/stable/topics/configuration/)
2. install awscli `sudo pip3 install awscli==1.18.105` , other older version might touble you. Refer [here](https://stackoverflow.com/questions/64596394/importerror-cannot-import-name-docevents-from-botocore-docs-bcdoc-in-aws-co)

**terraform**

1. as best practise set plugin cache as shown [here](https://www.scalefactory.com/blog/2021/02/25/terraform-plugin-caching/) 
2. set env for TF_WORKSPACE
3. set registry host as mentioned
4. TLS certs

