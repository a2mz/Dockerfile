FROM java:8-jre

MAINTAINER morozov <mx681121@gmail.com>

RUN wget http://download-aws.ej-technologies.com/jprofiler/jprofiler_linux_8_1_2.tar.gz -P /tmp/ && \
 tar -xzf /tmp/jprofiler_linux_8_1_2.tar.gz -C /usr/local &&\
 rm /tmp/jprofiler_linux_8_1_2.tar.gz

#ENV JPAGENT_PATH="-agentpath:/usr/local/jprofiler8/bin/linux-x64/libjprofilerti.so=nowait"
ENV JPAGENT_PATH="-agentpath:/usr/local/jprofiler8/bin/linux-x64/libjprofilerti.so=port=8849,nowait" 
EXPOSE 8849

CMD ["/bin/bash"]
