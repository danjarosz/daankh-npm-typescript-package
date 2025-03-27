# Daankh NPM Typescript Package Template

Template for creating typescript-based npm packages.

## Features

- Configured environment for creating and publishing NPM package
- Typescript support
- Prettier configuration for keep consistency in your code styling
- Vitest installation for writing tests of your modules

## How to use?

1. Clone the repository
2. Write your Typescript code in `src` directory.
3. Export the core content of your package in `src/index.ts` file.
4. Create `dev` branch to put your code there. To deploy the package make a pull request from `dev` into `main` branch.

## How to set up a package before start coding?

### package.json

Edit `package.json`:

```
{
    "name": <YOUR-PACKAGE-NAME>,
    "version": <INITIAL-PACKAGE-VERSION>,
    "description": <YOUR-PACKAGE-DESCRIPTION>,
    "repository": {
        "url": <URL-TO-YOUR-REPOSITORY>
    },
    "author": <YOUR-NAME>,
    "bugs": {
        "url": "<YOU-WHERE-REPORT-BUGS>"
    },
    "homepage": "<URL-TO-PACKAGE-HOMEPAGE>",
}
```

## How to deploy?

1. Ensure you're logged in your NPM account
   ```
   npm whoami
   ```
2. If you're not authenticated, log on your NPM account:
   ```
   npm login
   ```
3. Add a changeset
   ```
   npx changeset
   ```
4. Commit your changes
5. Run the `local-release` script
   ```
   npm run local-release
   ```
6. Congratulations! You're package is released! You can visit a page of your package:
   ```
   http://npmjs.com/package/<YOUR-PACKAGE-NAME>
   ```
