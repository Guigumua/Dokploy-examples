FROM node:latest
WORKDIR /app
COPY ./* ./

RUN npm install -g pnpm --registry=https://registry.npmmirror.com
RUN pnpm i --registry=https://registry.npmmirror.com --frozen-lockfile && pnpm run build

CMD ['pnpm', 'run', 'start']
