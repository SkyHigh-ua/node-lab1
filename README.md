# Lab 1

## Task

Create project in GitHub with minimal code-quality checks and autodepoly

### Requirements

- new repo in GitHub
- initial empty commit
  ```
  git commit --allow-empty -m "Initial commit"
  npm init
  ```
- add ESlint (as strict as possible)
  ```
  npm install eslint --save-dev
  npm init @eslint/config -- --config semistandard --config standard
  ```
- add Sonar-Lint to ESLint
  ```
  npm install eslint-plugin-sonarjs --save-dev --force
  ```
- add Prettier
  ```
  npm install --save-dev --save-exact prettier --force
  ```
- Add check on pre-commit hooks
  ```
  npx husky-init && npm install
  npx husky add .husky/pre-commit "npm run format"
  ```
- Add GitHub action to run checks\tests on commit or PR
- Add AutoDeployment to any hosting provider
- Add Editorconfig
