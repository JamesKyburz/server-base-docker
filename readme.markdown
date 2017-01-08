## Usage

# How to use this image

## npm

### Create a `Dockerfile` in your Node.js app project

```dockerfile
FROM jameskyburz/server-base-docker:latest
EXPOSE 8888
```

### Tell npm how to run your project in `package.json`
```javascript
"scripts": {
  "start": "node index"
}
```

## Yarn

### Create a `Dockerfile` in your Node.js app project

```dockerfile
FROM jameskyburz/server-base-docker:yarn
EXPOSE 8888
```

### Tell yarn how to run your project in `package.json`
```javascript
"scripts": {
  "start": "node index"
}
```

### When using yarn you will need to create a `yarn.lock` file

## Running

You can then build and run the Docker image:

```console
$ docker build -t my-nodejs-app .
$ docker run -it --rm --name my-running-app my-nodejs-app
```
