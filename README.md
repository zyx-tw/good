# good

A digital guaiguai at good.zyx.tw: the snack that engineers tape onto servers so they behave.

## Development

```sh
bun install
cp .env.example .env.local
bun run dev
```

## Checks

```sh
bun run typecheck && bun run lint && bun run format:check
```

## Deploy

ci builds the image in the pull request; a merge to main ships it to VM 117 through land (`.github/workflows/release.yml`). The stack lives in `/opt/good` with `compose.yaml` and `.env` (see `.env.example`).

## License

MIT
