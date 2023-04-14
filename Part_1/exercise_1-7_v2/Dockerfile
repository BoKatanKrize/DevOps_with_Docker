# Start from the ubuntu image v20.04
FROM ubuntu:20.04

# Use /usr/src/app as our workdir
WORKDIR /usr/src/app

# Install curl into the resulting image
RUN apt-get update
RUN apt-get -y install curl

# Copy the script.sh file from this location to /usr/src/app/
COPY script.sh .

# Add execution permissions
RUN chmod +x script.sh

# When running docker run the command ./script.sh
ENTRYPOINT ["./script.sh"]
