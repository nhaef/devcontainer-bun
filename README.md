🚀 Bun Dev Container
---------------------

This repository provides a development environment for [Bun](https://bun.sh/) using Visual Studio Code's [Dev Containers](https://containers.dev/).

## About Bun

Bun is a fast JavaScript all-in-one toolkit designed for developing, testing, running, and bundling JavaScript and TypeScript projects.
This Dev Container setup streamlines the development process by providing a pre-configured environment.

## Prerequisites

Before you begin, make sure you have the following tools installed on your system:
* [Visual Studio Code](https://code.visualstudio.com/)
* [Docker](https://www.docker.com/)

## Getting Started

To quickly set up your Bun development environment, follow these simple steps:

1. Open your project folder in Visual Studio Code.
2. In your project's root directory, create a `.devcontainer` folder if it doesn't already exist.
3. Inside the `.devcontainer` folder, create a `devcontainer.json` file.
4. Copy and paste the following configuration into your `devcontainer.json`:

```json
{
    "name": "Bun",
    "image": "ghcr.io/nhaef/devcontainer-bun:latest",
    "customizations": {
        "vscode": {
            "extensions": [
                "dbaeumer.vscode-eslint"
            ]
        }
    }
}
```

Once you have saved the `devcontainer.json` file,
Visual Studio Code should prompt you to reopen the project in a Dev Container.
Accept the prompt to set up the development environment inside a Docker container.
If you don't see the prompt,
you can access the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette),
type `Dev Containers: Reopen in Container`
and then press Enter.

Once the Dev Container is built and started, you'll have a fully configured environment for Bun development.

## Additional Information

For more information on Bun, check out the official [Bun documentation](https://bun.sh/docs).

If you encounter any issues or have questions, please feel free to [open an issue](https://github.com/nhaef/devcontainer-bun/issues/new) in this repository.

For more information on Visual Studio Code DevContainers, refer to the [official documentation](https://code.visualstudio.com/docs/devcontainers/containers).

## License

This project is licensed under the MIT License.