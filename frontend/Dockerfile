FROM node:18-slim

ENV TZ Asia/Tokyo

WORKDIR /frontend

RUN npm install -g pnpm

COPY . /frontend

RUN rm -rf .git/
RUN rm -rf node_modules

RUN pnpm install

# RUN npx nuxi upgrade --force

EXPOSE 3000

# CMD ["pnpm", "dev"]
