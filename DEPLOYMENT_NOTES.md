# OWASP Juice Shop - Deployment Notes

## Project

OWASP Juice Shop

## Environment

- OS: Windows 11
- Node.js: 24.21.0
- npm: 11.x

## Setup

1. Cloned the repository from GitHub.
2. Installed project dependencies using `npm install`.
3. Built the frontend.
4. Built the TypeScript server.
5. Started the application using `npm start`.

## Local Deployment

The application successfully runs locally on:

http://localhost:3000

## Troubleshooting

The initial frontend build failed because the installed Node.js version
(v22.11.0) did not satisfy the Angular CLI requirement.

Node.js was upgraded to v24.21.0.

After upgrading Node.js, the frontend and server compiled successfully.

The frontend SBOM generation step reported a missing
`dist/frontend/stats.json` metafile, but this did not prevent the
compiled application from starting successfully with `npm start`.