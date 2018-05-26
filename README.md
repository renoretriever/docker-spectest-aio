# Docker spectest aio

Specification test tool all in one.

## Testing tool

- [Serverspec](https://serverspec.org/)
- [awspec](https://github.com/k1LoW/awspec)
- [infrataster](https://github.com/ryotarai/infrataster)
- [goss](https://github.com/aelsabbahy/goss)

## Docker

- docker build

    ```
    $ docker build --no-cache --rm -t renoretriever/docker-spectest-aio .
    ```

## Serverspec

- initialize

    ```
    $ docker run -it --rm -v $(pwd):/root/ renoretriever/docker-spectest-aio serverspec-init
    ```

- execute

    ```
    $ docker run -it --rm -v $(pwd):/root/ -v ~/.ssh/:/root/.ssh/ renoretriever/docker-spectest-aio rake spec
    ```

## awspec

- version

    ```
    $ docker run --rm -it renoretriever/docker-spectest-aio awspec --version
    1.5.2
    ```

## infrataster

- initialize

    ```
    $ docker run -it --rm -v (pwd):/root/ -v ~/.ssh/:/root/.ssh/ renoretriever/docker-spectest-aio rspec --init
    ```

- execute

    ```
    $ docker run -it --rm -v (pwd):/root/ -v ~/.ssh/:/root/.ssh/ renoretriever/docker-spectest-aio rspec 
    ```

## goss

- version

    ```
    $ docker run --rm -it renoretriever/docker-spectest-aio goss --version
    goss version v0.3.5
    ```

