# Curriculum Notes
---
## Managing Packages with NPM

In `package.json` the `"dependecies"` field holds all required external packages. 'Dependacy Managment'.

Semantic versioning = `"package": "MAJOR.MINOR.PATCH"`

MAJOR changes increment when incomatble API changes are made.

MINOR changes are when backwards-compatible functionality is added. Does not break.

PATCH changes are backwards-compatible bug fixes. Does not break.

`~` prefix in version number keeps dependecy up to date with latest PATCH version.
`^` prefix in version numbers allows npm to install the latest PATCH and MINOR changes.

## Basic Node and Express

Express routes are handeled by creating an express object and using the following structure:
`app.METHOD(PATH, HANDLER).` Where: 

MTHOD is the http method.

PATH is the relative path on the server.

HANDLER is a function that express calls when a route is matched.

You can send files using `res.sendFile(file_path)` (this can be used to sexrve html).

`.env` files are hidden, only visible server side. Useful for keeping secrets and such. 
`.env` files are accessed using `process.env.VAR_NAME`.

MIDDLEWEARE functions take OBJECT, RESPONSE, and NEXT FUNCTION as arguments. Where NEXT FUNCTION is comma separated in route args.

ROUTE PARAMETERS look like this `route_path: '/user/:userId/book/:bookId' ` where words prefixed with `:` and delemited by `/` are the parameters. Those can be found in `req.params`.

QUERY PARAMETERS are added at the end of a route delemited by `?` and are found in `req.query`
