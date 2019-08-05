FROM rocker/rstudio


RUN apt-get update
RUN apt-get install -y --no-install-recommends \
    ed \
    default-jdk \
    icedtea-netx \
    libbz2-dev \
    libcairo2-dev \
    libgdal-dev \
    libicu-dev \
    liblzma-dev \
    libproj-dev \
    libgeos-dev \
    libgsl0-dev \
    librdf0-dev \
    librsvg2-dev \
    libv8-dev \
    libxcb1-dev \
    libxdmcp-dev \
    libxslt1-dev \
    libxt-dev \
    mdbtools \
    netcdf-bin \
  && . /etc/environment \
  && install2.r --error --repos $MRAN --deps TRUE \
    rJava devtools tidyr reshape2 dplyr DAAG bit64 zoo sqldf RJDBC \
  && R CMD javareconf \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/ \
  && rm -rf /tmp/downloaded_packages/ /tmp/*.rds