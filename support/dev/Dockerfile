# matches https://pages.github.com/versions
# pinned to sha for reproducability
FROM ruby:2.5.8@sha256:26d49fd3b2d22b11249b0161d7f7e8cbae8e1e0a22d1b76fd6c3ac017d4efc3e

 # ruby base doesn't specify locale https://github.com/docker-library/ruby/issues/45
ENV LANG C.UTF-8

# hadolint ignore=DL3008
RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    hunspell \
 && rm -rf /var/lib/apt/lists/*
