FROM node:20-slim 

RUN useradd -m -s /bin/bash test

WORKDIR /home/app
COPY package*.json ./

RUN npm install --omit=dev && npm install typescript

COPY . .

RUN npx tsc

RUN chown -R test:test /home/app
USER test

CMD ["node", "./build/index.js"]
