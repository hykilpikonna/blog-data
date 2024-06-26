# blog-data

Syncronized telegram channel data for my blog, created using my [TelegramBackup](https://github.com/one-among-us/TelegramBackup) project.

## Usage

1. Fork this repo (uncheck the option "Copy the _main_ branch only")
2. Create your secrets (read here: [TelegramBackup](https://github.com/one-among-us/TelegramBackup))
3. Run GitHub actions
4. Go to GitHub Pages settings and enable it, select `gh-pages` branch.
5. Your channel json will be hosted at `https://<username>.github.io/TelegramChanApi/posts.json`

(The GitHub actions script will update the JSON once every two hours)

### Timezone

If you need to change the time zone of the generated time, you can add the following information to the tgc yml file. You can click on [this link](https://github.com/jecanac474/blog-data/blob/main/.github/workflows/tgc.yml) to see an example of using Asia/Shanghai time zone.

```
env:
  TZ: Asia/Shanghai
  LC_TIME: POSIX
```

## Example

https://profile-api.hydev.org/posts.json

# Zotero API Localization

Additionally, this repo can be used to localize your Zotero publications. Just go to Settings > Secrets and put your Zotero user id into a secret named ZOTERO_USERID.
