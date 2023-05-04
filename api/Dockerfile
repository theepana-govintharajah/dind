FROM docker:23.0-dind
WORKDIR /app
COPY package*.json ./
RUN apk add --update nodejs yarn && \
    yarn install
COPY . .
EXPOSE 3000
CMD ["yarn", "start"]






# sudo docker run -it --rm node /bin/bash -c 'node --version'