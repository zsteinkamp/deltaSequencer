# deltaSequencer

A sequencer based on applying changes to a base pattern.

## Running
```
docker compose run app
```

## Developing
```
docker compose run dev
```

## Installing NPM Modules

To install a new NPM module, first stop your dev container. To do this, run (in another terminal window):
```
docker compose down
```
Then you can run the npm command this way:
```
docker compose run dev npm install --save my-cool-module
```
NPM will do its thing inside the container, and afterward you will see that the `package.json` and `package-lock.json` files have been updated.

Now rebuild the container:
```
docker compose build
```
And then bring up the dev container again:
```
docker compose run dev
```
