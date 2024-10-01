# retag-gha

This repository is an example of a GitHub workflow that moves the major `@V` tag based on the latest semantic versioning (semver) tag. This can be useful for actions or workflows where users expect the major version tag to point to the latest release.

## Workflow Explanation

The workflow updates the major version tag to point to the latest semver tag. For example, if the latest semver tag is `v1.2.3`, the `v1` tag will be moved to that commit.

## Example Usage

1. Clone the repository:
    ```sh
    git clone git@github.com:AlexB02/retag-gha.git
    cd retag-gha
    ```

2. Push a new semver tag:
    ```sh
    git tag v1.2.3
    git push origin v1.2.3
    ```
    or publish a new release on GitHub with the `v1.2.3` tag.

3. The GitHub Actions workflow will automatically update the `v1` tag to point to the `v1.2.3` commit.

## License

This project is licensed under the MIT License, feel free to use however you wish.