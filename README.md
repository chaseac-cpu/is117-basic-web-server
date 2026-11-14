# Chase's IS117 Web Server

Completed Express server and three required HTTP tests for IS117.

Repository to submit: https://github.com/chaseac-cpu/is117-basic-web-server

## Run

Requires Node.js 22 or newer.

```sh
npm ci
npm test
npm start
```

Visit http://localhost:3000. Press Ctrl+C to stop the server.

## Required tests

`npm test` runs `tests/server.test.js`, which starts and stops its own server:

1. `/` returns status 200 and the ROAM homepage as HTML.
2. `/about` returns status 200 and the ROAM about page as HTML.
3. `/missing-page` returns status 404 and `Page not found.`.

The root `index.js` exports and starts the completed app in
`is117-web-server/index.js`. Student pages and assets are in
`is117-web-server/public`.

## Additional development work

`npm run dev` starts the live reload development server.
The student app also includes a classroom message API and additional tests;
run those separately with `npm --prefix is117-web-server test` after installing
that folder's dependencies with `npm --prefix is117-web-server ci`.

The instructor's reference lessons and course maintenance tools have been
removed from this submission. The original course is credited in the Git
history; this repository contains Chase's completed student application.
