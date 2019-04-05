# playRStudio

## play RStudio in Docker Container

```
docker run -d -p 8787:8787 -v $(pwd):/home/rstudio -e PASSWORD=yourpasswordhere rocker/rstudio

```
