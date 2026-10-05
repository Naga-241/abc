# gh-operational-planning-webapp-ui

Built with React and TypeScript - Bundled with Vite - Utilizing CPrime
components

### Local Setup

1. **Repo setup and Git commands**

- To clone this repo, run:

  ```bash
    git clone https://github.com/Toyota-Motor-North-America/gh-operational-planning-webapp-ui.git
  ```

- Move to the develop branch
  ```
    git checkout develop
    git pull
  ```

2. **Pre-requisites**

- Install NodeJS version >= 20.
- Connect to latest version of Prime on Artifactory
  - Navigate to the
    [latest version of Prime on Artifactory](https://artifactory.tmna-devops.com/).
  - Login with GitHub SSO
  - Select the button labeled "Set Me Up" underneath your account avatar.
  - Click on npm
  - Select Repository: `npm-dev` and hit `Generate Token & Create Instructions`
  - Copy the content from Edit .npmrc (Unscoped), create a new file named
    `.npmrc` in the repo, and paste the content into it.

    ```
      email =
      always-auth = true
      registry=https://artifactory.tmna-devops.com/artifactory/api/npm/npm-prod/
      //artifactory.tmna-devops.com/artifactory/api/npm/npm-prod/:_authToken=
    ```

3. **Local Setup**

- At the root of the project directory, install project dependencies by running:

  ```
    npm install
  ```

- Once dependencies are installed, run:
  ```
    npm run dev
  ```

### Test Coverage

- Generate tests with coverage:

  ```bash
  npm run test
  ```

- Coverage outputs are written to the `coverage/` folder, including:
  - `coverage/lcov.info` (used by SonarQube)
  - `coverage/index.html` (open in a browser for the interactive report)
