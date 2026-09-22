# Mothscilla

A classical DAW for the browser — multitrack timeline, piano roll, sample-accurate
scheduling, automation, and a built-in FX/instrument library — built on
[`@synflow/core`](https://github.com/k1ln/synflow), the Synflow audio engine.

## Getting started

`@synflow/core` is vendored as a git submodule, not a copy — Mothscilla always
builds against the real engine source from the [synflow](https://github.com/k1ln/synflow)
repo.

```sh
git clone --recurse-submodules https://github.com/k1ln/mothscilla.git
cd mothscilla
npm install     # also builds the vendored @synflow/core
npm run dev
```

To pull in engine updates later:

```sh
git submodule update --remote synflow
npm install
```

## Scripts

- `npm run dev` — start the dev server
- `npm run build` — production build
- `npm test` — run the test suite
- `npm run gen:flows` — regenerate the built-in flow library

## License

AGPL-3.0-or-later — see [LICENSE](LICENSE). Free to use, study, modify, and share;
if you run a modified version as a network service, you must offer its source to
users of that service.
