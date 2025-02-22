# Nuxt Minimal Starter

## Essential Documentation

- [vue-tg Documentation](https://github.com/deptyped/vue-telegram) - Vue.js wrapper for Telegram Mini Apps
- [Telegram Mini Apps Documentation](https://core.telegram.org/bots/webapps) - Official Telegram Mini Apps development guide
- [Nuxt Documentation](https://nuxt.com/docs/getting-started/introduction) - Learn more about Nuxt.js

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

## Configuring Allowed Hosts

To prevent errors when using Telegram Mini App with ngrok or other tunneling services, make sure to add your allowed hosts in `nuxt.config.ts`:

```ts
export default defineNuxtConfig({
  vite: {
    server: {
      allowedHosts: ['.ngrok-free.app'] // Add your domain here
    }
  }
})
```
