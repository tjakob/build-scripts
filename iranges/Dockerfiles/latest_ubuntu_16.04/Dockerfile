#https://github.com/Bioconductor-mirror/Biobase.git
FROM ppc64le/r-base
MAINTAINER "Yugandha deshpande <yugandha@us.ibm.com>"

RUN apt-get update \
        && R -e 'source("https://bioconductor.org/biocLite.R"); biocLite("IRanges")' \
        && R CMD check IRanges

CMD ["/bin/bash"]
