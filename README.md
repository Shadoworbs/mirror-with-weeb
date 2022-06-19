# DEPLOY:

### STEP - 1:
Fork This Repo with all branches or use public template.

### STEP - 2:
Create config.env file using this template. [config_sample.env](https://raw.githubusercontent.com/codewithweeb/mirror-with-weeb/master/config_sample.env).

Fill `UPSTREAM_REPO` & `UPSTREAM_BRANCH` env vars else all these features won't be there !
`UPSTREAM_BRANCH` should be dev
Don't Use `ACCOUNTS_ZIP_URL` & `TOKEN_PICKLE_URL` (Broken for dev branch). Upload accounts folder & token.pickle files in heroku branch

### STEP - 3:
Fill All Action Secrets.

- `HEROKU_API`: Get it from your heroku account.
- `HEROKU_APP_NAME`: Set unique appname.
- `HEROKU_EMAIL`: Heroku Email ID
- `CONFIG_FILE_URL`: Optional ENV.. You can upload config.env on gist or in heroku branch

### STEP - 4:
RUN workflow with heroku branch from GitHub Action section !

## IMPORTANT ! :

For the simplification I've made some terms..

- `UNIFIED` = AppDrive, DriveApp, GDFlix, DriveBit, DriveLinks, DriveSharer, DriveAce, DrivePro, DriveFlix, DriveRoot, IndiDrive, AniDrive, DriveHub(in) Sharer Links
- `UNIFIED_EMAIL`: USE SAME GMAIL ACCOUNT IN ABOVE MENTIONED SHARERS
- `UNIFIED_PASS` : USE SAME PASSWORD IN ABOVE MENTIONED SHARERS

- `HUBDRIVE_CRYPT`: IT WILL BE USED TO BYPASS HUBDRIVE LINKS ONLY.
- `KATDRIVE_CRYPT`: IT WILL BE USED TO BYPASS KATDRIVE, KOLOP, DRIVEHUB(ws) LINKS.
- `DRIVEFIRE_CRYPT`: IT WILL BE USED TO BYPASS DRIVEFIRE & DRIVEBUZZ LINKS.

- `XSRF_TOKEN` & `laravel_session`: BOTH COOKIES WILL BE USED TO BYPASS SHARER.PW LINKS.

## CREDITS:
- [Maverick](https://github.com/majnurangeela) for integration and compatibility fixes
- [xcscxr](https://github.com/xcscxr) for his wonderful google drive link scrapers !
- [arata74](https://github.com/arata74) or [ANIME-REPUBLIC](https://github.com/ANIME-REPUBLIC) For Base Repo
