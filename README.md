# Shh Links

A Raycast extension that pastes links into Discord as `[site](<url>)`, `[text](<url>)` or `<url>`, so Discord shows no preview embed. See [extension/README.md](extension/README.md) for what it does and how to use it.

## Layout

- `extension/`: the extension itself, exactly what goes to the Raycast Store.
- `test/`: tests for the formatting logic. They live outside `extension/` because the Store does not accept tests in an extension.

## Development

```sh
cd extension
npm ci
npm run dev       # load it in Raycast while you edit
npm run build     # install the distribution build
npm run publish   # open or update the Store pull request
```

Run the tests from the repository root (Node 22.18 or later, which runs TypeScript directly):

```sh
npm test
```
