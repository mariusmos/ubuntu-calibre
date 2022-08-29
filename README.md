# ubuntu-calibre

Step 1:  Build a working XCFE image with the latest ubunut packages
  -> in progress
  Build command: docker build -f Dockerfile-xrdp.ubuntu -t ubu-image .
  
  Push to docker hub: 
    docker push marmos/ubuntu-desktop:tagname
    
  Running command:
    #docker run -it -p 33890:3389 marmos/ubuntu-desktop:latest testuser 1234 yes
    docker run -it -p 33890:3389 ubu-image:latest testuser 1234 yes
    
Step 2: Build a working image with Calibre Server incorporated

Step 3: Integrate in a compose file with the Calibre WEB Service shared


