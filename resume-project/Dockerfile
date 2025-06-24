FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
  texlive-latex-recommended \
  texlive-fonts-recommended \
  texlive-latex-extra \
  texlive-fonts-extra \
  texlive-lang-cyrillic \
  cm-super \
  make \
  && apt-get clean

WORKDIR /cv

COPY CV/ /cv/

RUN pdflatex -interaction=nonstopmode main.tex