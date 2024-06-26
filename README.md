# Ditto <a href="https://pokeapi.co/api/v2/pokemon/ditto"><img src='https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/132.svg' height='50px'/></a> [![PyPI - Version](https://img.shields.io/pypi/v/pokeapi-ditto)](https://pypi.org/project/pokeapi-ditto/)

This repository contains:

 - `ditto clone`: a script to crawl an instance of PokeAPI and download all data
 - `ditto analyze`: a script to generate a JSON schema of the above data
 - `ditto transform`: a script to apply a new base url to the above data and schema

## Usage

```sh
pip install pokeapi-ditto
ditto --help
```

## Development

```sh
poetry install
poetry run ditto --help
```

## Docker

You should have a PokeApi server running on `localhost:80`.

```sh
# runs clone, analyze, and transform all in one step
docker-compose up --build
```
