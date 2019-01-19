FROM kbuonforte/todobackend-base:latest
MAINTAINER Ken Buonforte <kbuonforte@gmail.com>

# Copy application artifacts
COPY target /wheelhouse
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse