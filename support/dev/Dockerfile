# matches https://pages.github.com/versions
# pinned to sha for reproducability
FROM ruby:2.7.3@sha256:c4cea7e31130d2a5db09dc65eb8884d79f215cf7f49c01723d488a0c7be1e965

 # ruby base doesn’t specify locale https://github.com/docker-library/ruby/issues/45
ENV LANG C.UTF-8

# hadolint ignore=DL3008
RUN apt-get update \
 && apt-get install -y --no-install-recommends \
    hunspell \
 && rm -rf /var/lib/apt/lists/*
