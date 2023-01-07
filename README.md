
# Hadolint for Dockerfile 

Hadolint is linter for Dockerfiles, it is checking if dockerfile has correct syntax (and that dockerfile is compliant with other defined rules)

official  GitRepo link  -[Hadolint](https://github.com/hadolint/hadolint#install)

official  site link  -[Hadolint](https://www.containiq.com/post/hadolint)

- Docker images should be efficient and secure.


### Installation steps
 LINUX
 
 step-1 
  -  wget -O /bin/hadolint https://github.com/hadolint/hadolint/releases/download/v2.12.0/hadolint-Linux-x86_64

  - download the newest version from official hadolint github [link](https://github.com/hadolint/hadolint/releases/)

  - chmod +x /bin/hadolint

  - verify the Installation ( hadolint --help )

 step-2
  - create Dockerfile
  - Hadolint syntex check [Rules](https://github.com/hadolint/hadolint#rules) 
  - In that folder 
  
  ```
   #Type this cmd 
   hadolint Dockerfile
   
   #if you want to ignore particular Rules 
   hadolint --ignore DL4000 -- ignore DL3042 Dockerfile
   
   #this cmd only shows error violations
   hadolint -t error Dockerfile

   
  ```

  ## Docker 
    
 Docker image [link](https://hub.docker.com/r/hadolint/hadolint)

 steps
  - create Dockerfile 
  - pull the docker hadolint image 
  ```
  docker pull hadolint/hadolint
  docker run --rm -i hadolint/hadolint < Dockerfile
  ```
  


  ## Reference link
   - [link-1](https://www.youtube.com/watch?v=bj73gCDz8aU)
   - [link-2](https://godatadriven.com/blog/lint-your-dockerfile-with-hadolint/)
  




