<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/3830bd5f-a9e7-425f-b9ce-6bb52d30785a

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Deploy to GitHub Pages

This project is configured to deploy automatically to GitHub Pages from the `main` branch.

1. Push this repo to GitHub.
2. In GitHub, go to `Settings > Pages`.
3. Under `Build and deployment`, select `GitHub Actions` as the source.
4. Push to `main` or run the `Deploy to GitHub Pages` workflow manually from the `Actions` tab.

After the workflow finishes, the demo will be published at:

`https://<your-user>.github.io/<your-repo>/`

Notes:

- The Vite `base` path is adjusted automatically for GitHub Pages project URLs.
- Right now the app is effectively static, so GitHub Pages is a good fit.
- If you later add real Gemini requests in the browser, do not expose a private API key in the frontend.
