FROM ubuntu:18.04

# Update apt
RUN apt-get update -y

# Install deps
RUN apt-get install -y python3 python3-pip 
RUN python3 -m pip install setuptools
RUN apt-get install -y texlive-latex-base texlive-fonts-recommended texlive-fonts-extra texlive-latex-extra
RUN apt-get install -y texlive-bibtex-extra biber
RUN apt-get install -y pandoc pandoc-citeproc