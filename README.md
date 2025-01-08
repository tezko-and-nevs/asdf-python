# exec-block

opinionated linter for config files. yaml, json, toml.

```
npm i -g exec-block
```

check files:

```
exec-block check config.yaml
```

rules:

- no tabs (use spaces)
- consistent quotes
- sorted keys (optional)
- trailing commas
- max line length 120

### auto-fix

```
exec-block fix config.yaml
```

### ci integration

```yaml
# .github/workflows/lint.yml
- run: exec-block check *.{yaml,json,toml}
```

### disable rules

```yaml
# .exec-block.yaml
rules:
  sorted-keys: false
  max-line-length: 200
```

exit code 0 if pass, 1 if fail.

MIT • made for prettier doesn't handle yaml well

# Touch update: 1761209118
