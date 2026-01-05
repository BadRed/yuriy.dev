# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
| `npm run deploy`          | Build and deploy to Cloudflare Pages             |

## 🚢 Automatic Deployment to Cloudflare Pages

This project is configured to automatically deploy to Cloudflare Pages when you push to the `main` branch.

### Setup Instructions

1. **Get your Cloudflare API Token:**
   - Go to [Cloudflare Dashboard](https://dash.cloudflare.com/profile/api-tokens)
   - Create a new API Token with "Cloudflare Pages" permissions
   - Copy the token

2. **Get your Cloudflare Account ID:**
   - Go to [Cloudflare Dashboard](https://dash.cloudflare.com)
   - Select your account
   - Copy the Account ID from the right sidebar

3. **Add secrets to your GitHub repository:**
   - Go to your repository settings on GitHub
   - Navigate to Settings > Secrets and variables > Actions
   - Add the following repository secrets:
     - `CLOUDFLARE_API_TOKEN`: Your Cloudflare API token
     - `CLOUDFLARE_ACCOUNT_ID`: Your Cloudflare Account ID

4. **Push to main:**
   - Once secrets are configured, any push to the `main` branch will trigger an automatic deployment
   - Check the Actions tab in your GitHub repository to monitor the deployment

### Manual Deployment

You can also deploy manually using:
```sh
npm run deploy
```

This requires the Wrangler CLI to be authenticated with your Cloudflare account.

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
