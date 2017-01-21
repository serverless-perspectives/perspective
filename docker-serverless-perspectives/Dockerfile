FROM haskell

MAINTAINER Jack Warner <jack.warner@parivedasolutions.com>

# will ease up the update process
# updating this env variable will trigger the automatic build of the Docker image
ENV PANDOC_VERSION "1.19.1"

# install pandoc
RUN cabal update && cabal install pandoc-${PANDOC_VERSION}

RUN cabal install pandoc-citeproc

# install latex packages
RUN apt-get update -y \
  && apt-get install -y --no-install-recommends \
    texlive-latex-base \
    texlive-xetex latex-xcolor \
    texlive-math-extra \
    texlive-latex-extra \
    texlive-fonts-extra \
    texlive-bibtex-extra \
    fontconfig \
    lmodern

WORKDIR /source

RUN apt-get install -y --no-install-recommends \
    git

RUN git clone https://github.com/citation-style-language/styles.git /styles

ENTRYPOINT ["/root/.cabal/bin/pandoc"]

CMD ["--help"]
