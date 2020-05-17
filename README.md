![Mastodon](https://i.imgur.com/NhZc40l.png)
====

View the documentation at <https://docs.joinmastodon.org>

### Build/Deploy

#### Requires
* Hugo 

(on macOS: `brew install hugo`\
 windows: `choco install hugo -confirm`\
 linux: `apt-get install hugo` OR `snap install hugo`)


#### build the static site
`hugo -D` 

Output will be in `./public/` 

TODO clean up the ad hoc quick and dirty doc copy, for now:

```bash
cp -R ./public/* ../public/docs
cp -R ../public/docs/*{.svg,.png} ../public/
mv ../public/docs/assets/ ../public/assets
cp -R ../public/docs/docs/* ../public/docs
```

This hack will copy the static files into ../public/docs, and then copy the ./public/docs/ folder content into ../public/docs as well so we can route to the static files properly (There is 100% an easy fix that will allow for this hack to be removed, but for now it works.)

