# Repository Guidelines

## Project Structure & Module Organization

LinkForge is planned as a React and Express full-stack application. The current repository contains project documentation in `Reame.md`; application folders may be added as the project is implemented.

- `client/` — React application, including UI components, pages, styles, and frontend assets.
- `server/` — Express API, routes, middleware, and backend services.
- `.env` files — local configuration only. Keep them inside the relevant application folder and never commit them.

Keep frontend and backend dependencies isolated in their respective `package.json` files. Place reusable frontend components under a clear feature or `components/` directory, and group Express routes with the code they serve.

## Build, Test, and Development Commands

Run commands from the applicable application directory after it exists:

```bash
cd client && npm install       # install React dependencies
cd client && npm start         # start the React development server
cd client && npm run build     # create a production frontend build
cd server && npm install       # install Express dependencies
cd server && npm run dev       # start the API in development mode
```

The frontend is expected at `http://localhost:3000`; configure the backend port (for example, `PORT=5000`) through `server/.env`.

## Coding Style & Naming Conventions

Use 2-space indentation for JavaScript, JSON, and CSS. Prefer `const`, async/await, and small single-purpose functions. Name React components in PascalCase (`LinkCard.jsx`), hooks with `use` (`useLinks.js`), and variables/functions in camelCase. Use descriptive route paths such as `/api/links`. Add a formatter or linter configuration before applying style-only bulk changes; none is configured yet.

## Testing Guidelines

No test framework or coverage threshold is configured currently. When adding tests, keep them near the feature or use a dedicated `tests/` directory, name them `*.test.js` or `*.test.jsx`, and add a documented `npm test` script. Cover successful requests, validation failures, and key UI states.

## Commit & Pull Request Guidelines

The repository currently has only the `Initial commit` baseline, so use short imperative commit subjects, for example `Add link validation`. Keep commits focused. Pull requests should explain the change, link relevant issues, list verification steps, and include screenshots for visible UI changes. Do not include secrets, `.env` files, or generated dependency folders.
