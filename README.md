# whitehawk-external-mastercard-riskrecon-api

## What

Generates various language stub code from swagger specifications.

- [v0/cpe](https://api.riskrecon.com/v0/cpe/swagger)
- [v1](https://api.riskrecon.com/v1/swagger)
- [v2](https://api.riskrecon.com/v2/swagger)

## Trigger Release

```bash
pnpm run release
git push --follow-tags
```

This will cause the [build.yml](./.github/workflows/build.yml) to be executed.

## Building (manual)

### Build language-specific artifacts

```bash
.ci/all-ci build $(git describe)
```

### Publish language-specific artifacts

```bash
.ci/all-ci publish
```

## Learning Resources

### Git

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/#summary)
