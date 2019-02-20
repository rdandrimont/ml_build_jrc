# ml_build_jrc
machine learning build for docker

0. !!!IF NOT SUDO WITH FULL PERMISSIONS!!! Before building the dockerfile make the working directory (/data) accessible to the R container by running this command inside EACH directory:

   chmod -R 777 <dir>

1. Mount volume to container 

   docker run -it -p 8787:8787 -v /data/:/data <IMAGE ID>

2. Disable browser plugins Rstudio in order to access terminal - 

   Tools -> Global options -> Terminal -> uncheck "Connect with WebSockets"
