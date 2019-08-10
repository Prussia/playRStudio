# playRStudio

## play RStudio in Docker Container

```
$ mkdir -p ~/container/rstudio && cd ~/container/rstudio

$ docker run -d -p 8787:8787 --name rstudio \
                                            -v $(pwd):/home/rstudio \
                                            -e ROOT=TRUE \
                                            #-e ADD=shiny \
                                            -e PASSWORD=<PASSWORD> \
                                            -e USER=<CUSTOM_NAME> \
                                            prussia2016/playrstudio
                                            #rocker/rstudio
```
```
install.packages('txtplot')
```

## R Programming

### https://www.w3cschool.cn/r/
### https://www.katacoda.com/basiafusinska/courses/r-basics

## Learning Roadmap

### [RStudio Essentials](https://www.rstudio.com/resources/webinars/#849ed0fea538d4329)

- Programming Part 1 (Writing code in RStudio)
- Programming Part 2 (Debugging code in RStudio)
- Programming Part 3 (Package writing in RStudio)
- Managing Change Part 1 (Projects in RStudio)
- Managing Change Part 2 (Github and RStudio)
