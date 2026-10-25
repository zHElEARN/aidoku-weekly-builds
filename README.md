# aidoku-weekly-builds

Weekly build of [Aidoku](https://github.com/Aidoku/Aidoku) `main` with the `com.zhelearn.Aidoku`
bundle identifier, published as an AltStore/Feather source.

## Source

```
https://raw.githubusercontent.com/zHElEARN/aidoku-weekly-builds/main/app-repo.json
```

## How it runs

- Every Monday 00:00 UTC, or manually via **Actions → Build Aidoku (Weekly) → Run workflow**
- Skips when `main` has not moved since the last successful build; tick `force` to rebuild anyway
- Publishes a `weekly-YYYY.MM.DD` release and rewrites `app-repo.json` with that single version
- Keeps the last 3 releases

## Output

- `Aidoku.ipa` — unsigned, sign it with your own certificate
- Bundle identifier `com.zhelearn.Aidoku`, iCloud container `iCloud.com.zhelearn.Aidoku`
