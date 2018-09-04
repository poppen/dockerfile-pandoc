# Docker Pandoc

Docker container with texlive and pandoc.

## Usage

In the container, the workdir is set `/src`. So mount the directory which contains markdowns you want to convert to `/src`.

For example:

    docker run --rm -v `pwd`:/src -it poppen/pandoc sample.md -o sample.pdf --latex-engine=lualatex -V documentclass=ltjarticle -V geometry:a4paper -V geometry:margin=1in
