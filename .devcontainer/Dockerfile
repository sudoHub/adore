FROM mcr.microsoft.com/devcontainers/typescript-node:1-22-bullseye

RUN apt-get update && apt-get install -y deno
RUN apt-get update && apt-get install -y ubuntu-24.04-desktop

RUN mkdir /workspace
WORKDIR /workspace

# Install Nuxt 3
RUN npm install -g nuxi

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install