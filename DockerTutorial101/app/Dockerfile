FROM node:12-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
#  The CMD directive specifies the default command to run when starting a container from this image.
CMD ["node", "src/index.js"]