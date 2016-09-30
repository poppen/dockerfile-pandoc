# Docker Pandoc

Ubuntu 16.04 container with texlive and pandoc packages.

## Usage

Pandoc always be run from the /src directory in the container.

    docker run --rm -v `pwd`:/src -it poppen/pandoc sample.md -o sample.pdf --latex-engine=lualatex -V documentclass=ltjarticle -V geometry:a4paper -V geometry:margin=1in
