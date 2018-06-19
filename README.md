# nk_croc
Character recognition and object classification system for images

## Quick Start

Use CROC in your project via pip with `pip3 install -e <path/to/croc>`.

or

Start CROC as a service on your local-machine with:

1) `docker build -t croc-api:dev -f ./api.dockerfile .`
2) `docker run -p 5000:5000 croc-api:dev`

## Structure of this repo

The core of this repo is `setup.py` and `nk_croc`. 

This repo is pip-installsable and makes the contents of `nk_croc` available after installation.

There is an api-wrapper for the library located in `api-wrapper`. It uses `nk_croc` and can be built with the `api.dockerfile`. For more information see [the README.md in `api-wrapper`](./api-wrapper/README.md)

## Coming soon

- Other wrappers for croc that are segmented out in other repos?
