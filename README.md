<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1WYfGVBkC_yGzSnrDt5ddjpZcdoMsQiJl

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `VITE_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## Troubleshooting

- **TypeScript cannot find Node typings** (`Cannot find type definition file for 'node'`):
  Run `npm install --include=dev` to reinstall dependencies (including `@types/node`) before building with `npm run build`. If you previously ran installs with production-only flags such as `--omit=dev`, rerun the install without them so the typings are restored.
