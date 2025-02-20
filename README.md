# ollama-container

podman-compose setup for ollama and deepseek-r1:7b

## Setup

Run `./up` instead of `podman-compose up -d` since [podman-compose doesn't support compose.yml post_start commands](https://github.com/containers/podman/issues/25370)

Note that the `deepseek-r1` model is pulled asynchronously.  Wait for `./up` (`podman-compose exec`) to finish before trying to use the command line or web UI.