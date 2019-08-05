FROM rocker/rstudio


apt-get install -y --no-install-recommends \
    ed \
    default-jdk \

    ## Install Alpla Dependencies: ggplot2 provided by verse image
        && install2.r --error --repos $MRAN --deps TRUE \
        rJava devtools tidyr reshape2 dplyr DAAG bit64 zoo sqldf RJDBC \

    ## Reconfigure Java R
      && R CMD javareconf \
      && apt-get clean \
      && rm -rf /var/lib/apt/lists/ \
      && rm -rf /tmp/downloaded_packages/ /tmp/*.rds