# NgNeat Elf Documentation Archive

Unofficial restored documentation archive for [NgNeat Elf](https://www.npmjs.com/package/@ngneat/elf) and related packages.

The original public `ngneat/elf` repository and `https://ngneat.github.io/elf/` documentation are no longer reliable, while the npm packages are still available and may still be used by existing projects.

This repository keeps a deployable copy of the archived Docusaurus docs so teams maintaining Elf-based applications can keep a stable reference.

## What This Contains

This is the full Elf Docusaurus docs app copied from [`ngneat-archive/elf`, branch `restore/npm-elf-cli-3.1.1`](https://github.com/ngneat-archive/elf/tree/restore/npm-elf-cli-3.1.1/docs).

It was not reduced to a small subset. The archive includes the broader Elf documentation: store, repository/facade patterns, entities, requests, requests result, pagination, persist state, history, devtools, immer, CLI, side effects, miscellaneous APIs, recipes, troubleshooting, and third-party docs such as `elf-sync-state`.

The branch name comes from the archive restoration branch. Even though it references `elf-cli`, the package manifests in that branch provide a useful version snapshot for the Elf packages listed below.

## Version Snapshot

| Package | Version | Source |
| --- | --- | --- |
| `@ngneat/elf` | `2.5.1` | [`packages/store/package.json`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/packages/store/package.json) |
| `@ngneat/elf-entities` | `5.0.2` | [`packages/entities/package.json`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/packages/entities/package.json) |
| `@ngneat/elf-requests` | `1.9.2` | [`packages/requests/package.json`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/packages/requests/package.json) |
| `@ngneat/elf-persist-state` | `1.2.1` | [`packages/persist-state/package.json`](https://github.com/ngneat-archive/elf/blob/restore/npm-elf-cli-3.1.1/packages/persist-state/package.json) |
| `@ngneat/error-tailor` | `5.0.1` | [`ngneat-archive/error-tailor`](https://github.com/ngneat-archive/error-tailor/tree/restore/npm-error-tailor-5.0.1) |
| `elf-sync-state` | `1.3.0` | [`RicardoJBarrios/elf-sync-state`](https://github.com/RicardoJBarrios/elf-sync-state) |

The first four packages above are verified directly from the archived Elf monorepo branch. `@ngneat/error-tailor` is restored from its separate archive. `elf-sync-state` is documented from its own repository and the third-party page included in the Elf docs archive.

If your project depends on similar Elf versions, this archive may be useful as a historical reference. It is not an official continuation of NgNeat Elf.

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
