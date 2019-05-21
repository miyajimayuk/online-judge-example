FROM ubuntu:16.04
RUN apt-get update -y \
  && apt-get install -y curl zip unzip sudo tar tzdata \
  && apt-get clean
RUN apt-get -y install ruby
RUN apt-get -y install python
RUN apt-get -y install time
RUN apt-get -y install binutils

CMD su nobody

RUN curl -s https://get.sdkman.io | bash
RUN /bin/bash -l -c "source ~/.sdkman/bin/sdkman-init.sh;sdk install java;sdk install kotlin;sdk install gradle"

ENV PATH $PATH:~/.sdkman/candidates/java/current/bin
ENV PATH $PATH:~/.sdkman/candidates/kotlin/current/bin

CMD /bin/bash