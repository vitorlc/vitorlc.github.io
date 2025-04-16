# Currículo Vitae #
  [Vitor de Lima Cirqueira](https://vitorlc.github.io)

# Build the Docker image
docker build -t resume-template .

# Run the container
docker run --rm --name resume-template -v "$PWD":/home/app --network host resume-template

# With not work
docker run --rm --name resume-template -p 4000:4000 -v "$PWD":/home/app resume-template bundle exec jekyll serve --host 0.0.0.0 --force_polling
