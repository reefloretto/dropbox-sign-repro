# README

Steps to reproduce "module not found" error in the `@dropbox/sign` package:

- Clone this repo
- Run `yarn` to install dependencies
- Run `yarn build` to build the package
- Notice the error

The errors look something like:

```
@reefloretto ➜ /workspaces/dropbox-sign-repro (main) $ yarn build
yarn run v1.22.19
$ next build
   ▲ Next.js 14.0.1

Failed to compile.

./node_modules/@dropbox/sign/dist/api.js
Module not found: Can't resolve './aes'

https://nextjs.org/docs/messages/module-not-found

Import trace for requested module:
./app/dropbox/page.tsx

./node_modules/@dropbox/sign/dist/api.js
Module not found: Can't resolve './blowfish'

https://nextjs.org/docs/messages/module-not-found

Import trace for requested module:
./app/dropbox/page.tsx

./node_modules/@dropbox/sign/dist/api.js
Module not found: Can't resolve './cipher-core'

https://nextjs.org/docs/messages/module-not-found

Import trace for requested module:
./app/dropbox/page.tsx

./node_modules/@dropbox/sign/dist/api.js
Module not found: Can't resolve './core'

https://nextjs.org/docs/messages/module-not-found

Import trace for requested module:
./app/dropbox/page.tsx

./node_modules/@dropbox/sign/dist/api.js
Module not found: Can't resolve './enc-base64'

https://nextjs.org/docs/messages/module-not-found

Import trace for requested module:
./app/dropbox/page.tsx


> Build failed because of webpack errors
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
