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
