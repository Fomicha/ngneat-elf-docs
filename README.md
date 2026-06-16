# NgNeat Elf Docs Archive

Restored documentation for the Elf-related packages used by our application.

The original public `ngneat/elf` repository and `https://ngneat.github.io/elf/` docs are no longer reliable, while the npm packages are still used in the main project. This repository keeps a deployable Docusaurus copy of the docs that match our dependency versions.

## Covered Packages

| Package | Version | Source |
| --- | --- | --- |
| `@ngneat/elf` | `2.5.1` | [`ngneat-archive/elf`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1) |
| `@ngneat/elf-entities` | `5.0.2` | [`ngneat-archive/elf`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1) |
| `@ngneat/elf-requests` | `1.9.2` | [`ngneat-archive/elf`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1) |
| `@ngneat/elf-persist-state` | `1.2.1` | [`ngneat-archive/elf`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1) |
| `@ngneat/error-tailor` | `5.0.1` | [`ngneat-archive/error-tailor`](https://github.com/ngneat-archive/error-tailor/tree/restore/npm-error-tailor-5.0.1) |
| `elf-sync-state` | `1.3.0` | [`RicardoJBarrios/elf-sync-state`](https://github.com/RicardoJBarrios/elf-sync-state) |

## Important Source Pages

- Elf docs app: [`ngneat-archive/elf/docs`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1/docs)
- Store: [`store.mdx`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/docs/docs/store.mdx)
- Entities: [`entities.mdx`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/docs/docs/features/entities-management/entities.mdx)
- Requests status/cache/data source: [`requests`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1/docs/docs/features/requests)
- Requests result: [`requests-result.mdx`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/docs/docs/features/requests-result.mdx)
- Persist state: [`persist-state.mdx`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/docs/docs/features/persist-state.mdx)
- Sync state: [`sync-state.mdx`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/docs/docs/third-party/sync-state.mdx)
- Error Tailor README: [`ngneat-archive/error-tailor/README.md`](https://github.com/ngneat-archive/error-tailor/blob/restore/npm-error-tailor-5.0.1/README.md)

## Local Development

```bash
cd docs
npm ci
npm run start
```

## Build

```bash
cd docs
npm ci
npm run build
```

## Railway

Railway service settings:

```txt
Root Directory: docs
Build Command: npm ci && npm run build
Start Command: npm run serve -- --host 0.0.0.0 --port $PORT
```

The Docusaurus `baseUrl` is configured as `/`, so the Railway deployment should work from the root of the generated domain.

