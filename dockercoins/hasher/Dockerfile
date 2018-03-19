FROM ruby:2.5-slim-stretch
RUN apt-get update \
  && apt-get install -y build-essential \
  && rm -rf /var/lib/apt/lists/*
RUN gem install sinatra
RUN gem install thin
ADD hasher.rb /
CMD ["ruby", "hasher.rb"]
EXPOSE 80
