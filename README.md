# Base Project

This project forked from [https://github.com/5hay/notionbackup](https://github.com/5hay/notionbackup)

## How To Use

Set the following env variables
- Create setting csv.(See. **Setting file**)
- `NOTION_TOKEN` (the token_v2 cookie value, just google "notion token_v2")
- _Optional_ `NOTION_EXPORTDIR` (the folder where the created .zip file should be placed in, **defaults to the current directory**)
  - Only specify the directory, the filename will be created for you
- _Optional_ `NOTION_EXPORTTYPE` ("html" or "markdown", **defaults to markdown**)

Now you can just run `./notionbackup [export_setting_csv]`.

## Setting file

See. backup_pages.csv
- `formatType` ( csv )
- `colume` : page_name,page_id 

## Building
See. [https://github.com/5hay/notionbackup](https://github.com/5hay/notionbackup)
```
go build -o notionbackup -ldflags="-s -w" app.go
```

## Special Thanks

-  [https://github.com/5hay/notionbackup](https://github.com/5hay/notionbackup)
