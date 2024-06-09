# My Project

![Unit Tests](https://github.com/om-chevli/BCDV4033/actions/workflows/unit-tests.yml/badge.svg)

## Unit Test Workflow

This project uses GitHub Actions to automate the testing process. The unit test workflow runs every time changes are pushed to the repository. It ensures that all unit tests pass before the changes are merged into the main branch.

### Video Link
https://youtu.be/PZLrEZ8O-1o

### Workflow Details

- **Name**: Unit Test Workflow
- **Trigger**: After the build process is completed.
- **Steps**:
  - Checkout the code.
  - Set up Node.js.
  - Install dependencies.
  - Run Jest tests.

### Commit Tag

To indicate the status of the unit tests in your commits, add the following badge to your commit messages:

![Unit Tests](https://github.com/om-chevli/BCDV4033/actions/workflows/unit-tests.yml/badge.svg)
