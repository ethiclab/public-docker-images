FROM ethiclab/node-xsltproc:1.0
USER root
RUN echo "Fix behaviour on accepting model.xml and initial state concatenated from standard input." && \
git clone https://github.com/ethiclab/modelc /tmp/modelc
WORKDIR /tmp/modelc/template
