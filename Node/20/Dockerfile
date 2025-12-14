FROM node:20-alpine
RUN apk add --no-cache bash curl
WORKDIR /app/data
CMD ["sh", "-c", "if [ -f package.json ]; then echo 'Starting'; npm install --production && node index.js; else echo 'No package.json found, container idle'; tail -f /dev/null; fi"]
