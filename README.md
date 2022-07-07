# Hello world javascript action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

### `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

## Outputs

### `time`

The time we greeted you.

## Example usage

uses: actions/hello-world-javascript-action@v1.1
with:
  who-to-greet: 'Mona the Octocat'

## Contributions

In an effort to remove node modules from the repository, this project depends on on `@vercel/ncc` to compile all modules and our source code into one single `index.js` file found in `dist/`. Thus all changes to `index.js` needs to be compiled with the following command: `ncc build index.js --license licenses.txt`.