FROM docker:23.0-dind
WORKDIR /app
COPY package*.json ./
RUN apk add --update nodejs yarn && \
    yarn install
COPY . .
EXPOSE 3000
CMD ["yarn", "start"]






# In terminal run the following commands
# sudo docker build -t image2:latest .
# sudo docker run -p 3000:3000 image2