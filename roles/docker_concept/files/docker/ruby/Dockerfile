#
# Ruby Dockerfile
#
# https://github.com/dockerfile/ruby
#

# Pull base image.
FROM dockerfile/ubuntu

# Install Ruby.
# RUN \
#   apt-get update && \
#   apt-get install -y ruby ruby-dev ruby-bundler && \
#   rm -rf /var/lib/apt/lists/*

RUN mkdir -p /root/.ssh/

ADD app.deploy /root/.ssh/
ADD config /root/.ssh/
RUN chmod 700 /root/.ssh/app.deploy
# Define working directory.
# WORKDIR /data
# RUN git clone git@github.com:shopsmart/wwwproxy.git /home/wwwproxy

# Define default command.
CMD ["bash"]
