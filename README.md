# Docker Formatter
Docker images for formatting code for different languages



## Build docker image

```docker build -t black-formatter .```

## Run black formatter

```
docker run --rm -v $(pwd)/format:/code black-formatter /code/test.py
```

- `$(pwd)/format:/code:` Mounts the local format directory to the /code directory inside the container.
- `black-formatter`. The name of the Docker image to run.
- `/code/test.py` The path to the file to format inside the container.

