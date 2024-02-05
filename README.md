# Example of sharing code between `model` and `web` packages

The `userName` function is exported from `model` and imported into `web` in `main.ts`

Some things to make sure:

- moduleResolution in `tsconfig.json` of web is "bundler"
- The `tsconfig.json` of the `model` package has settings that work in node and browser environments
- The `exports` field is set in the `model` package
- I couldn't get this to work with an `npm install`, `yarn`, `pnpm` or `bun` should work
