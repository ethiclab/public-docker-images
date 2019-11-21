FROM ethiclab/node-xsltproc:1.0
USER root
RUN echo "Fix #13 - Precision is lost from one interaction to another." && \
echo "https://github.com/ethiclab/modelc/issues/13" && \
echo "commit 024819b (HEAD -> master, origin/master, origin/HEAD) Use the hex format of doubles." && \
git clone https://github.com/ethiclab/modelc /tmp/modelc
WORKDIR /tmp/modelc
RUN npm run new-model abc
WORKDIR /tmp/modelc/model_abc
RUN make test && ./model
