FROM rocker/binder:4.2.3
LABEL maintainer='Safia Read'
COPY --chown=${NB_USER} . ${HOME}
USER ${NB_USER}



RUN wget https://github.com/safiaread/Data-Science-Project-Template/raw/main/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2023-04-06/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
