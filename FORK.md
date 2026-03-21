# Fork Notes

Fork of [riba2534/feishu-cli](https://github.com/riba2534/feishu-cli).

## Local Changes

### `local` branch

| Change | File | Description |
|--------|------|-------------|
| Default to Device Flow | `cmd/auth_login.go` | `auth login` defaults to `--method device` (RFC 8628), no redirect URL config needed |

## Sync Workflow

```bash
git fetch upstream
git checkout main && git merge upstream/main
git checkout local && git merge main
git push origin local
```
