FROM debian

MAINTAINER ehaggon <ehaggon@student.21-school.ru>

RUN apt-get update && apt-get install -y git
RUN git clone https://github.com/ilovetostudyit/shell_scripts.git
RUN cd shell_scripts && git pull
RUN apt install -yq bash
ENTRYPOINT bash shell_scripts/cows.sh

# How to build it?
# docker build -it a00 .

# How to run it?
# docker run --rm -ti a00