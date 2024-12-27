# vue-lhci

## Project Setup

### Build the development docker image

```sh
docker build -t vue-lhci -f ./Dockerfile.dev .
```

### Install dependencies

```sh
docker run --rm -v $(pwd):/app vue-lhci npm install
```

### Start dev server

```sh
docker run -it --rm -v $(pwd):/app -p 8080:8080 vue-lhci npm run dev
```
