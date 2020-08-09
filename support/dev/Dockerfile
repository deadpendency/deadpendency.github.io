# matches https://pages.github.com/versions
# pinned to sha for reproducability
FROM ruby:2.7.1@sha256:4cdd89e947cc52c78c273953e42a6e9d94ca4cd182875fd50745550580b772f4

 # ruby base doesn’t specify locale https://github.com/docker-library/ruby/issues/45
ENV LANG C.UTF-8

# hadolint ignore=DL3008
RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    hunspell \
 && rm -rf /var/lib/apt/lists/*
