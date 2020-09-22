FROM ubuntu:18.04

# Update apt
RUN apt-get update -y

# Fix a TZData issue
RUN ln -snf /usr/share/zoneinfo/$(curl https://ipapi.co/timezone) /etc/localtime

# Install deps
RUN apt-get install -y python3 python3-pip 
RUN python3 -m pip install setuptools
RUN apt-get install -y texlive-latex-base texlive-fonts-recommended texlive-fonts-extra texlive-latex-extra
RUN apt-get install -y texlive-bibtex-extra biber
RUN apt-get install -y pandoc pandoc-citeproc