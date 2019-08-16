FROM ethiclab/node-xsltproc:1.0
USER root
RUN git clone https://github.com/ethiclab/modelc /tmp/modelc
WORKDIR /tmp/modelc
RUN npm run new-model abc
WORKDIR /tmp/modelc/model_abc
RUN make test && ./model > result.js && node result.js && cat result.js
