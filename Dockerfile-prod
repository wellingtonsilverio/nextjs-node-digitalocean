FROM node:14

WORKDIR /usr/src/app
COPY frontend/package*.json ./
RUN yarn cache clean && yarn --update-checksums
COPY ./frontend ./
EXPOSE 3000
RUN yarn build
CMD ["yarn", "start"]