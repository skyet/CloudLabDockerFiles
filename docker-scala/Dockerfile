FROM yinlu0053/java8
MAINTAINER ylu0053

# install scala 2.10.4, requires libjansi-java
RUN apt-get install libjansi-java; \
    wget http://www.scala-lang.org/files/archive/scala-2.10.4.deb; \
    dpkg -i scala-2.10.3.deb; \
    rm -f scala-2.10.4.deb

# cleanup temp files
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
