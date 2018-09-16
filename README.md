# docker-rust-wasm

Preinstalled dependencies for https://rustwasm.github.io/book/game-of-life/setup.html

## Usage

```
docker run -v "$PWD":/usr/src/myapp -w /usr/src/myapp --rm --interactive --tty stereobooster/rust-wasm
USER=<user name> cargo generate --git https://github.com/rustwasm/wasm-pack-template
cd <project name>
wasm-pack init
```

## Development

```
docker build -t rust-wasm .
docker tag rust-wasm stereobooster/rust-wasm
docker push stereobooster/rust-wasm
```