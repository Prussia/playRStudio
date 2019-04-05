# playRStudio

## play RStudio in Docker Container

```
$ mkdir -p ~/container/rstudio && cd ~/container/rstudio

$ docker run -d -p 8787:8787 -v $(pwd):/home/rstudio -e PASSWORD=pazzword rocker/rstudio

```
