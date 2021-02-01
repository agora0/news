---
layout: page
permalink: /readme/
---

Read news on demand.

| Source | Importer  | Update |
| ------ | --------- | ------ |
| BBC    | RSSBBC    | 5/Day  |
| CNA    | RSSCNA    | 5/Day  |
| DW     | RSSDW     | 5/Day  |
| JOINS  | RSSJOINS  | 5/Day  |
| KYODO  | RSSKYODO  | 5/Day  |
| REUTERS| RSSREUTERS| 5/Day  |
| RFI    | RSSRFI    | 5/Day  |
| RTHK   | RSSRTHK   | 5/Day  |

## Test and Deploy

```
$ gem install bundler jekyll 
$ vim _config.yml # Configure to test or deploy.

$ bundle exec jekyll serve
# => Now browse to http://localhost:4000

$ JEKYLL_ENV=production bundle exec jekyll build
# Copy the compiled codes from _site/ to html server.
```

## List of Features

- [x] Batch and Automate - Check out the [issue comment](https://github.com/agorahub/news0/issues/1#issuecomment-597540617)

## Disclaimer

The information and opinions within this website are for information purposes only. They are not intended to constitute legal or other professional advice, and should not be relied on or treated as a substitute for specific advice relevant to particular circumstances. We accept no responsibility for any errors, omissions or misleading statements on this website, or for any loss which may arise from reliance on materials contained on this website. Certain parts of this site may link to external Internet sites, and other external Internet sites may link to this website. We are not responsible for the content of any external Internet sites.

