# LinkForge

LinkForge is a full-stack web application built with **React.js** on the frontend and **Express.js** on the backend.

## Tech Stack

- **Frontend:** React.js
- **Backend:** Node.js and Express.js
- **Package manager:** npm

## Project Structure

```text
LinkForge/
├── client/             # React application
├── server/             # Express API
└── Reame.md
```

## Getting Started

### Prerequisites

Install the following before running the project:

- [Node.js](https://nodejs.org/) (version 18 or later recommended)
- npm (included with Node.js)

### Install dependencies

Install the frontend dependencies:

```bash
cd client
npm install
```

Install the backend dependencies:

```bash
cd ../server
npm install
```

### Run the application

Start the Express server:

```bash
cd server
npm run dev
```

In a separate terminal, start the React application:

```bash
cd client
npm start
```

The React app is commonly available at `http://localhost:3000`. Configure the Express server port and API URL in the project as needed.

## Environment Variables

Keep private configuration in a `.env` file in the relevant application directory. Do not commit `.env` files to version control.

Example backend variables:

```env
PORT=5000
```

## Available Scripts

Typical scripts used by this project include:

```bash
npm start       # Run the React development server
npm run dev     # Run the Express server in development mode
npm run build   # Create a production React build
```

Refer to each application's `package.json` for the exact scripts available.

## License

Add license information here.
