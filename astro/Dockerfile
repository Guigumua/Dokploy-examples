FROM node:18

COPY ./* ./

RUN npm install -g pnpm --registry=https://registry.npmmirror.com
RUN pnpm i --registry=https://registry.npmmirror.com && pnpm run build

CMD ['pnpm', 'run', 'start']
