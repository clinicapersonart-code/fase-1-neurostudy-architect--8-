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
4. Pull the latest changes (for example in VS Code: **Source Control > ... > Pull**):
   `git pull origin main`

5. If there were updates after pulling, reinstall deps (only if `package.json` or lockfiles changed):
   `npm install`
6. Verify the project still builds:
   `npm run build`

> Tip (VS Code): You can open an integrated terminal with ``Ctrl+` `` and run the commands above without leaving the editor. Merge conflicts will appear in the Source Control view with inline accept options.

## Troubleshooting

- **TypeScript cannot find Node typings** (`Cannot find type definition file for 'node'`):
  `@types/node` now installs with the rest of the dependencies. If you still see this error, rerun `npm install` (without `--omit=dev` or `--production`) so the typings are restored before `npm run build`.
