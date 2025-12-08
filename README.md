# Code with GitHub Copilot

_Learn to code faster with AI-powered suggestions using GitHub Copilot in VS Code and Codespaces._

[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-enabled-blue.svg)](https://github.com/features/actions)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Table of Contents

- [About](#about)
- [Workflows](#workflows)
- [Technology Stack](#technology-stack)
- [Step 1: Leverage Codespaces with VS Code for Copilot](#step-1-leverage-codespaces-with-vs-code-for-copilot)
- [Step 2: JavaScript Skills](#step-2-javascript-skills)
- [Step 3: Copilot Hub](#step-3-copilot-hub)
- [Step 4: Copilot Comments](#step-4-copilot-comments)
- [Step 5: Review and Improve Suggestions](#step-5-review-and-improve-suggestions)
- [Step 6: Testing & Validation](#step-6-testing--validation)
- [Step 7: Completion](#step-7-completion)
- [Contributing](#contributing)
- [License](#license)

## About

This repository is a GitHub Skills course that teaches developers how to leverage GitHub Copilot for AI-powered code suggestions. GitHub Copilot helps you write code faster by offering autocomplete-style suggestions right in VS Code and Codespaces.

Key features include:

- **Interactive Learning**: Step-by-step course using GitHub Actions to track progress
- **GitHub Codespaces Integration**: Practice Copilot in a cloud-based development environment
- **Hands-on Examples**: Real coding exercises with JavaScript and development containers
- **Automated Workflows**: GitHub Actions workflows guide learners through each step

## Workflows

This repository includes five simple example workflows in `.github/workflows` that demonstrate different aspects of the learning experience:

- **Auto Assign** (`auto-assign.yml`): Example workflow for repository automation
- **Copilot Extension Setup** (`copilot-extension-setup.yml`): Example workflow for extension configuration
- **JavaScript Skills** (`javascript-skills.yml`): Example workflow for JavaScript practice
- **Copilot Hub** (`copilot-hub.yml`): Example workflow for advanced Copilot features
- **Copilot Comments** (`copilot-comments.yml`): Example workflow for comment-based code generation

These workflows are provided as simple examples referenced in the README to demonstrate GitHub Actions integration.

## Technology Stack

This course uses the following technologies:

- **HTML5**: For web-based content and examples
- **Primer CSS**: GitHub's design system for consistent styling
- **http-server (npm)**: Simple local development server for testing web content
- **GitHub Actions**: Workflow automation and course progression tracking
- **GitHub Codespaces**: Cloud-based development environment with pre-configured settings
- **VS Code**: Primary code editor with integrated Copilot support

## Step 1: Leverage Codespaces with VS Code for Copilot

_Welcome to "Develop With AI Powered Code Suggestions Using GitHub Copilot and VS Code"! :wave:_

GitHub Copilot is an AI pair programmer that helps you write code faster and with less work. It draws context from comments and code to suggest individual lines and whole functions instantly. GitHub Copilot is powered by OpenAI Codex, a generative pretrained language model created by OpenAI.

**Copilot works with many code editors including VS Code, Visual Studio, JetBrains IDE, and Neovim.**

Additionally, GitHub Copilot is trained on all languages that appear in public repositories. For each language, the quality of suggestions you receive may depend on the volume and diversity of training data for that language.

Using Copilot inside a Codespace shows just how easy it is to get up and running with GitHub's suite of [Collaborative Coding](https://github.com/features#features-collaboration) tools.

> **Note**
> This skills exercise will focus on leveraging GitHub Codespace. It is recommended that you complete the GitHub skill, [Codespaces](https://github.com/skills/code-with-codespaces), before moving forward with this exercise.

### :keyboard: Activity: Enable Copilot inside a Codespace

**We recommend opening another browser tab to work through the following activities so you can keep these instructions open for reference.**

Before you open up a codespace on a repository, you can create a development container and define specific extensions or configurations that will be used or installed in your codespace. Let's create this development container and add copilot to the list of extensions.

1. Navigating back to your **Code** tab of your repository, click the **Add file** drop-down button, and then click `Create new file`.

2. Type or paste the following in the empty text field prompt to name your file.

   ```
   .devcontainer/devcontainer.json
   ```

3. In the body of the new **.devcontainer/devcontainer.json** file, add the following content:

   ```json
   {
       "name": "Codespace for Skills!",
       "customizations": {
           "vscode": {
               "extensions": [
                   "GitHub.copilot"
               ]
           }
       }
   }
   ```

4. Select the option to **Commit directly to the `main` branch**, and then click the **Commit new file** button.

5. Navigate back to the home page of your repository by clicking the **Code** tab located at the top left of the screen.

6. Click the **Code** button located in the middle of the page.

7. Click the **Codespaces** tab on the box that pops up.

8. Click the **Create codespace on main** button.

   **Wait about 2 minutes for the codespace to spin itself up.**

9. Verify your codespace is running. The browser should contain a VS Code web-based editor and a terminal should be present such as the below:

   ![Screen Shot 2023-03-09 at 9 09 07 AM](https://user-images.githubusercontent.com/26442605/224102962-d0222578-3f10-4566-856d-8d59f28fcf2e.png)

10. The `copilot` extension should show up in the VS Code extension list. Click the extensions sidebar tab. You should see the following:

    ![Screen Shot 2023-03-09 at 9 04 13 AM](https://user-images.githubusercontent.com/26442605/224102514-7d6d2f51-f435-401d-a529-7bae3ae3e511.png)

**Wait about 60 seconds then refresh your repository landing page for the next step.**

## Step 2: JavaScript Skills

**Objective**: Create a JavaScript function in the `src/` directory and demonstrate basic usage or unit testing.

### :keyboard: Activity

1. In your Codespace, create a new directory called `src` if it doesn't exist.

2. Create a new file `src/skills.js` with a simple JavaScript function (use Copilot to help you write it).

3. Add example usage or a basic test to validate your function works.

4. Commit your changes to the repository.

**Validation**: Ensure your JavaScript file is created and the function can be executed or tested.

## Step 3: Copilot Hub

**Objective**: Explore GitHub Copilot's suggestion panel and accept at least one code suggestion.

### :keyboard: Activity

1. Open the Copilot panel in VS Code (click the Copilot icon in the Activity Bar on the left sidebar).

2. Start typing a comment describing what you want to code (e.g., `// function to calculate fibonacci sequence`).

3. Review the suggestions provided by Copilot.

4. Accept one of the suggestions by pressing `Tab` or clicking on it.

5. Test the generated code to ensure it works as expected.

**Validation**: Confirm that you've successfully accepted and tested a Copilot suggestion.

## Step 4: Copilot Comments

**Objective**: Use code comments to guide Copilot in generating function implementations.

### :keyboard: Activity

1. Create a new file or open an existing one in your `src/` directory.

2. Write a detailed comment describing a function you want to create (e.g., `// Create a function that validates email addresses using regex`).

3. Allow Copilot to suggest the implementation based on your comment.

4. Accept the completion and test the function.

5. Commit your changes.

**Validation**: Ensure the commented function was successfully completed by Copilot and works correctly.

## Step 5: Review and Improve Suggestions

**Objective**: Learn to evaluate and refactor code suggestions from Copilot for better quality.

### :keyboard: Activity

1. Review the code that Copilot has generated in previous steps.

2. Identify areas where the code could be improved (e.g., error handling, edge cases, performance).

3. Refactor the code to make it more robust and maintainable.

4. Add additional tests or validation to ensure the improved code works correctly.

5. Commit your improvements.

**Validation**: Verify that your refactored code is cleaner, more efficient, and handles edge cases properly.

## Step 6: Testing & Validation

**Objective**: Run a local development server and verify your examples work as expected.

### :keyboard: Activity

1. If you have HTML/CSS files, install and run `http-server`:

   ```bash
   npm install -g http-server
   http-server
   ```

2. Open the local server URL in your browser and verify your examples render correctly.

3. Test all JavaScript functions you've created to ensure they work properly.

4. Fix any issues you discover during testing.

5. Commit your final tested code.

**Validation**: Confirm that all examples work correctly when tested locally.

## Step 7: Completion

**Objective**: Create a pull request with all your changes and confirm automated checks pass.

### :keyboard: Activity

1. Ensure all your changes are committed to your branch.

2. Push your branch to GitHub.

3. Open a pull request from your branch to `main`.

4. Add a descriptive title and body to your PR explaining the changes you made.

5. Wait for any automated checks to run and ensure they pass.

6. Request a review if working in a team setting.

**Validation**: Confirm your PR is created, all checks pass, and the changes are ready for review.

Congratulations! You've completed the GitHub Copilot skills course! :tada:

## Contributing

Contributions are welcome! If you'd like to improve this course:

1. Fork the repository

2. Create a feature branch (`git checkout -b feature/improvement`)

3. Make your changes

4. Run any local checks to ensure your changes don't break existing functionality

5. Commit your changes (`git commit -m 'Add some improvement'`)

6. Push to the branch (`git push origin feature/improvement`)

7. Open a Pull Request

Please ensure your contributions align with the course objectives and maintain the educational value for learners.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Copyright (c) 2025 char23-web

---

## Help & Support

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/code-with-copilot) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

© 2025 char23-web &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)
