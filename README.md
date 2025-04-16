# Currículo Vitae #
  [Vitor de Lima Cirqueira](https://vitorlc.github.io)

# Build the Docker image
docker build -t resume-template .

# Run the container
docker run --rm --name resume-template -v "$PWD":/home/app --network host resume-template
