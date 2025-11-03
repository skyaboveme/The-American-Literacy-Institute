# The American Literacy Institute

A modern website built with Astro to promote literacy and education across America.

## 🚀 Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       ├── index.astro
│       ├── about.astro
│       ├── programs.astro
│       └── contact.astro
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |

## 📚 About This Project

This website serves as the online presence for The American Literacy Institute, featuring:

- **Home Page**: Welcome message and overview of our mission
- **About Page**: Organization history, values, and impact statistics
- **Programs Page**: Detailed information about our various literacy programs
- **Contact Page**: Contact information and inquiry form

## 🛠 Technology Stack

- **Astro**: Modern static site generator
- **TypeScript**: Type-safe JavaScript
- **CSS**: Custom styling with modern CSS features

## 🚀 Deployment

This site is configured to deploy to **theamericanliteracyinstitute.com** via GitHub Pages.

### Automatic Deployment Setup

The repository includes a GitHub Actions workflow that automatically builds and deploys the site when changes are pushed to the main branch.

#### Steps to Enable GitHub Pages:

1. **Enable GitHub Pages in Repository Settings:**
   - Go to your repository on GitHub
   - Navigate to Settings > Pages
   - Under "Build and deployment", select "GitHub Actions" as the source

2. **Configure Custom Domain:**
   - In the same GitHub Pages settings, under "Custom domain", enter: `theamericanliteracyinstitute.com`
   - Click "Save"
   - The CNAME file is already included in the `public/` directory

3. **Configure DNS Settings:**
   - In your domain registrar's DNS settings, add the following records:

   **For root domain (theamericanliteracyinstitute.com):**
   ```
   Type: A
   Name: @
   Value: 185.199.108.153

   Type: A
   Name: @
   Value: 185.199.109.153

   Type: A
   Name: @
   Value: 185.199.110.153

   Type: A
   Name: @
   Value: 185.199.111.153
   ```

   **For www subdomain (optional):**
   ```
   Type: CNAME
   Name: www
   Value: skyaboveme.github.io
   ```

4. **Enable HTTPS:**
   - After DNS propagation (may take up to 24 hours), return to GitHub Pages settings
   - Check the "Enforce HTTPS" option

### Manual Deployment

You can also build and deploy manually:

```bash
npm install
npm run build
# The built files will be in the ./dist/ directory
```

## 📖 Learn More

For more information about Astro, check out [the Astro documentation](https://docs.astro.build).

## 📝 License

All rights reserved - The American Literacy Institute
