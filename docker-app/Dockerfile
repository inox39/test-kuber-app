FROM ruby:alpine3.13
RUN apk add --update --no-cache libcap
COPY http_server /app
RUN setcap 'cap_net_bind_service=+ep' /usr/local/bin/ruby
USER 65534
WORKDIR /app
ENTRYPOINT ["ruby", "http_server.rb"]
