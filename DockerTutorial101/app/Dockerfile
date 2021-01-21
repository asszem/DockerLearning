FROM node:12-alpine
WORKDIR /app
#To avoid reinstall every time http://localhost/tutorial/image-building-best-practices/
COPY package.json yarn.lock ./ 
RUN yarn install --production
COPY . .
#  The CMD directive specifies the default command to run when starting a container from this image.
CMD ["node", "src/index.js"]