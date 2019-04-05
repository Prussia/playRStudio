# playRStudio

## play RStudio in Docker Container

```
$ mkdir -p ~/container/rstudio && cd ~/container/rstudio

$ docker run -d -p 8787:8787 --name rstudio ||
-v $(pwd):/home/rstudio || 
-e ROOT=TRUE ||
-e ADD=shiny || 
-e PASSWORD=<PASSWORD> ||
-e USER=<CUSTOM_NAME> rocker/rstudio

```

## 
