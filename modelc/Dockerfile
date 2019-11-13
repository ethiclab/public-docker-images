FROM ethiclab/node-xsltproc:1.0
USER root
RUN echo "Fix #11 - default test fails" && \
echo "commit 30188aef5046b283a48d0e70da10b9e2269ba93f" && \
git clone https://github.com/ethiclab/modelc /tmp/modelc
WORKDIR /tmp/modelc
RUN npm run new-model abc
WORKDIR /tmp/modelc/model_abc
RUN make test && ./model
