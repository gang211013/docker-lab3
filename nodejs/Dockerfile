FROM centos
MAINTAINER zhao yonggang <zhaoyg@test.com>

RUN yum install -y gcc gcc-c++ make python38
RUN yum install -y nodejs npm

ADD nodeapp /opt/nodeapp

WORKDIR /opt/nodeapp
RUN npm install

EXPOSE 3000

ENTRYPOINT [ "node", "server.js" ]
