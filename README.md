## Debian/Ubuntu Startup Script

See `debian-startup-script.sh`

## Cookie Format
`cookies-pointfree.txt` and `cookies-swifttalk.txt` should be present in the working dir and have the first line:

```
# Netscape HTTP Cookie File
```

## Google Drive Setup
- download `client_secrets.json` from Google Developer Console
- on the first attempt to upload you would be requested to authenticate
and the `credentials.json` file will be stored for subsequent use

## My notes
0. cd to the project root dir.
1. Run `pipenv install` to install dependencies
2. Prepare cookie file
	1. 在一个已经登录的browser里，把cookie导出来.
3. Double check the output folder:
	`self.VIDEOS_DIR = "/Volumes/t7-touch/PointFree"``
4. Double check the video resolution:
	`-f "best[height<=540]"`
4. Download: `pipenv run python3 ./grab.py --no-gdrive-upload`
