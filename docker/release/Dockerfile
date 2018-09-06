FROM louspringer/todobackend-base:latest
MAINTAINER Lou Springer <lou@louspringer.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse