FROM ruby:3.0

# throw errors if Gemfile has been modified since Gemfile.lock
#RUN bundle config --global frozen 1

WORKDIR /usr/src/myapp

# Copies ---

COPY Gemfile ./

COPY . .

# Run --

RUN bundle install

# Comandos a ejecutar -> descrito en el enunciado

CMD ["bundle", "exec", "rackup", "--host", "0.0.0.0", "-p", "4567"]


