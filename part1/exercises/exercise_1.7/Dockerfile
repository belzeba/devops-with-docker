# Start from the Ubuntu 20.04
FROM ubuntu:20.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the script.sh file with execute permission from this location to /usr/src/app/ creating /usr/src/app/script.sh
COPY --chmod=0755 script.sh .

# Update packages list, upgrade outdated packages and install curl
RUN apt update && apt upgrade -y && apt install curl -y

# When running Docker run the command will be ./script.sh
CMD ./script.sh
